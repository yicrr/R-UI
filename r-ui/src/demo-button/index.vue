<template>
  <button class="demo-button" :class="type">
    <slot />
  </button>
</template>

<script>
export default {
  name: 'DemoButton',

  props: {
    color: String,
    type: {
      type: String,
      default: 'primary',
    },
  },
};
</script>

<style lang="scss">
.demo-button {
  min-width: 120px;
  color: #fff;
  font-size: 16px;
  line-height: 36px;
  border: none;
  border-radius: 30px;
}
.demo-button:hover {
  opacity:0.8;
  cursor: pointer;
}
.primary {
  background-color: #f44;
}
.success {
  background-color: rgb(126, 198, 143);
}
.error {
  background-color: rgb(196, 110, 97);
}
</style>

<template>
  <input class="demo-button">
</template>

<script>
export default {
  name: 'DemoInput',

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
  background-color: #f44;
  border: none;
  border-radius: 30px;
}
</style>

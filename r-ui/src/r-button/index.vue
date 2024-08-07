<template>
    <button class="r-button">
      <slot />
    </button>
</template>
<script>
  export default {
    name: 'RButton',
  
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
  .r-button {
    min-width: 120px;
    color: #fff;
    font-size: 16px;
    line-height: 36px;
    background-color: #f44;
    border: none;
    border-radius: 30px;
  }
</style>
  
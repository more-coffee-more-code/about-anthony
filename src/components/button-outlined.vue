<template>
  <a :href=this.url target="_blank">
    <button class="button-outlined">Go to project ></button>
  </a>
</template>
<script>
export default {
  name: 'button-outlined',
  props: [
    'url'
  ]
}
</script>
<style lang="scss">

@import '../assets/global-styles.scss';
.button-outlined {
  border: 2px solid $color-material-white;
      background-color: black;
      color: $color-material-white;
      padding: 14px 28px;
      font-size: 16px;
      cursor: pointer;
      border-radius: 5px;
      margin: 2.5rem auto 0;
}
</style>

<template>
  <a :href=this.url :target=" (this.openNewTab) ? '_blank': '_self'">
    <button class="button-outlined">{{ this.buttonCopy}}</button>
  </a>
</template>
<script>
export default {
  name: 'button-outlined',
  props: {
    url: String,
    buttonCopy: String,
    openNewTab: Boolean
  }
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
      border-radius: 5px;
      margin: 2.5rem auto 0;
}

.button-outlined:hover {
  cursor: pointer;
}
</style>

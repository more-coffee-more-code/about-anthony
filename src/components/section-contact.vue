<template>
  <section class="section-contact">
    <div class="section-contact__content">
      <h1 class="section-contact__header">Contact me!</h1>
    </div>
  </section>
</template>
<script>
export default {
  name: 'section-contact'
}
</script>
<style lang="scss">
@import '../assets/global-styles.scss';

.section-contact {
  height: $section-height;

  &__content {

  }

  &__header {
    font-size: $section-header-font-size;
  }
}
</style>

<template>
  <section class="section-experience-dev">
    <div class="section-experience-dev__content">
      <h1 class="section-experience-dev__header">Developer xp</h1>
    </div>
  </section>
</template>
<script>
export default {
  name: 'section-experience-dev'
}
</script>
<style lang="scss">
@import '../assets/global-styles.scss';

.section-experience-dev {
  height: $section-height;

  &__header {
    font-size: $section-header-font-size;
  }
}
</style>

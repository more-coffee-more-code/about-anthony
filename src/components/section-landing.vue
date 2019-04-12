<template>
  <section class="section-landing">
    <div class="section-landing__content">
      <h1 class="section-landing__header">Anthony Ruffin</h1>
      <nav class="section-landing__nav">
        <a class="section-landing__nav__item" href="">Skills</a>
        <a class="section-landing__nav__item" href="">Developer</a>
        <a class="section-landing__nav__item" href="">Qa</a>
        <a class="section-landing__nav__item" href="">Contact</a>
      </nav>
    </div>
  </section>
</template>
<script>
export default {
  name: 'section-landing'
}
</script>
<style lang="scss">
@import '../assets/global-styles.scss';

.section-landing {
  height: $section-height;

  &__content {
    width: 100%;
    max-width: 600px;
    justify-content: center;
    align-content: center;
    margin: 0 auto;
  }

  &__header {
    font-size: $section-header-font-size;
    border-bottom: green solid 4px;
  }

  &__nav {
    display: flex;
    justify-content: space-evenly;
    
    &__item {
      color: #fafafa;
    }
  }
}
</style>

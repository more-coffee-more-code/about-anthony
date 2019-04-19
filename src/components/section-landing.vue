<template>
  <section class="section-landing">
    <div class="section-landing__content">
      <h1 class="section-landing__header">{{ this.header }}</h1>
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
  name: 'section-landing',
  data() {
    return {
      windowWidth: 0,
      windowHeight: 0
    }
  },
  created() {
    window.addEventListener('resize', this.handleResize);
    this.handleResize();
  },
  methods: {
    header() {
      this.handleResize();
      let lineBreak = (this.windowWidth > 900) ? 'Anthony Ruffin' : 'Anthony Ruffin'; 
      console.log(lineBreak);
      // return lineBreak; 
      return 'asdfasdf';
    },
    handleResize() {
      // console.log('resized');
      return this.windowWidth = window.innerWidth;
    }
  }
}
</script>
<style lang="scss">
@import '../assets/global-styles.scss';

.section-landing {
  height: $section-height;

  &__content {
    max-width: $section-landing-content-width;
    justify-content: center;
    align-content: center;
    margin: 0 auto;
  }

  &__header {
    font-size: $section-header-font-size;
    border-bottom: #9CCC65 solid 4px;
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

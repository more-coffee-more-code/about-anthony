<template>
  <section class="section-landing">
    <div class="section-landing__content">
      <h1 class="section-landing__header">Anthony Ruffin</h1>
      <div class="section-landing__nav">
        <nav-button class="section-landing__nav__item" 
          buttonCopy="Skills"
          url="#skills"
          :openNewTab="false"
        />
        <nav-button class="section-landing__nav__item" 
          buttonCopy="Developer"
          url="#developer"
          :openNewTab="false"
        />
        <nav-button class="section-landing__nav__item" 
          buttonCopy="QA"
          url="#qa"
          :openNewTab="false"
        />
        <nav-button class="section-landing__nav__item" 
          buttonCopy="Connect :)"
          url="#contact"
          :openNewTab="false"
        />
      </div>
    </div>
  </section>
</template>
<script>
import NavButton from '../components/button-outlined.vue';

export default {
  name: 'section-landing',
  components: {
    NavButton
  },
  data() {
    return {
      windowWidth: 0,
      windowHeight: 0
    }
  },
  methods: {

  }
}
</script>
<style lang="scss">
@import '../assets/global-styles.scss';

.section-landing {
  height: $section-height;
  display: flex;

  &__content {
    align-self: center;
    justify-content: space-evenly;
    margin: 0 auto;
  }

  &__header {
    margin: 0 auto;
    // max-width: $section-landing-content-width;  
    font-size: $section-header-font-size;
    color: $color-light-green;
  }

  &__nav {
    display: flex;
    margin: 0 auto;
    flex-direction: column;
    
    @include for-desktop {
      justify-content: space-evenly;
    }
    
    &__item {
      color: #fafafa;
    }
  }
}
</style>

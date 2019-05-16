<template>
  <section class="section-landing">
    <div class="section-landing__content">
      <h1 class="section-landing__header">{{ this.name }}</h1>
      <div class="section-landing__nav section-landing__nav--flex-edge">
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
          buttonCopy="Let's talk :)"
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
      windowHeight: 0,
      name: '<Anthony Ruffin />'
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
    font-size: $section-landing-header-font-size-mobile;
    color: $color-light-green;

    @include for-desktop {
      font-size: $section-header-font-size-desktop;
    }
  }

  &__nav {
    display: flex;
    margin: 0 auto;
    flex-direction: column;
    
    @include for-desktop {
      justify-content: space-evenly;
      flex-direction: row;
      
      @supports (-ms-accelerator: true) {
        &--flex-edge {
          justify-content: space-around;
        }
      } 
    }

    &__item {
      color: #fafafa;
    }
  }
}
</style>

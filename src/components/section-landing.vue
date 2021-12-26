<template>
  <section class="section-landing">
    <div class="section-landing__content">
      <h1 class="section-landing__header">{{ this.name }}</h1>
      <h3 class="section-landing__subheadline">{{ this.subheadline }}</h3>
    </div>
  </section>
</template>
<script>
export default {
  name: 'section-landing',
  data() {
    return {
      windowWidth: 0,
      windowHeight: 0,
      name: '<Anthony Ruffin />',
      subheadline: 'Designer. Developer. QA'
    }
  }
}
</script>
<style lang="scss">
@import '../assets/global-styles.scss';

.section-landing {
  min-height: $section-height;
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

  &__subheadline {
    font-size: 14px;
    color: #fafafa;

    @include for-desktop {
      font-size: 2rem;
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

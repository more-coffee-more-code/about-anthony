<template>
  <section class="section-experience-dev" id="developer">
    <div class="section-experience-dev__content">
      <h1 class="section-experience-dev__header">Developer</h1>
      <section class="section-experience-dev__experience-display">
        <div class="section-experience-dev__experience-display__wrapper">
        
        </div>
      </section>
    </div>
  </section>
</template>
<script>
import DevProject from '../components/project.vue';
import ButtonOutlined from '../components/button-outlined.vue';

export default {
  name: 'section-experience-dev',
  components: {
    DevProject,
    ButtonOutlined
  },
  data() {
    return {
      
    }
  }
}
</script>
<style lang="scss">
@import '../assets/global-styles.scss';

// todo: set section height on mobile to auto

.section-experience-dev {
  display: flex;
  height: auto;
  min-height: $section-min-height;

  @include for-desktop {
    height: $section-height;
    min-height: 100vh;
  }

  &__content {
    height: auto;
    margin: 0 auto;
    align-self: center;
  }

  &__header {
    display: inline-block;
    margin: 0 auto 4rem;
    border-bottom: $section-header-border-width solid #9CCC65;
    justify-content: center;
    font-size: $section-header-font-size-mobile;

    @include for-desktop {
      font-size: $section-header-font-size-desktop;
    }
  }

  &__experience-display {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    max-width: $section-content-max-width;
    margin: 0 auto;

    &__wrapper {
      max-width: 500px;
      min-height: 300px;
      height: 100%;
      margin: 0 auto;
    }

    &__experience {
      margin: 0 auto;
      white-space: pre-line;
    }
  }
}
</style>

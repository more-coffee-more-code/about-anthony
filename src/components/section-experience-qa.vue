<template>
  <section class="section-experience-qa" id="qa">
    <div class="section-experience-qa__content">
      <h1 class="section-experience-qa__header">QA</h1>
      <div class="section-experience-qa__experience-display">
        <div class="section-experience-qa__experience-display__wrapper">
          <qa-project
            title="Google shopping insights"
            description="Gain insight into how often products are searched"
            class="section-experience-qa__experience-display__experience"
          />
          <button-outlined
            class="section-experience-qa__experience-display__button"
            url="https://shopping.thinkwithgoogle.com/"
            buttonCopy="Go to project >"
            :openNewTab="true"
          />
        </div>
        <!-- todo: break project title -->
        <div class="section-experience-qa__experience-display__wrapper">
          <qa-project
            title="Assembly NFK"
            description="Designed to connect. New collaborative space in downtown Norfolk"
            class="section-experience-qa__experience-display__experience"
          />
          <button-outlined
            class="section-experience-qa__experience-display__button"
            buttonCopy="Go to project >"
            url="https://www.assemblynfk.com/"
            :openNewTab="true"
          />
        </div>
        <div class="section-experience-qa__experience-display__wrapper">
          <qa-project
            title="Think with Google - Mobile gaming"
            description="Gain insight into how to best monetize your mobile apps"
            class="section-experience-qa__experience-display__experience"
          />
          <button-outlined
            class="section-experience-qa__experience-display__button"
            buttonCopy="Go to project >"
            url="https://www.thinkwithgoogle.com/feature/mobile-gaming-genres/"
            :openNewTab="true"
          />
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import QaProject from '../components/project.vue';
import ButtonOutlined from '../components/button-outlined';

export default {
  name: 'section-experience-qa',
  components: {
    QaProject,
    ButtonOutlined
  }
}
</script>
<style lang="scss">
@import '../assets/global-styles.scss';

.section-experience-qa {
  height: auto;
  display: flex;
  min-height: $section-min-height;
  
  @include for-desktop {
    height: $section-height;
  }

  &__content {
    max-width: $section-content-max-width;
    margin: 0 auto;
    height: auto;
    align-self: center;
  }

  &__header {
    margin: 0 auto 4rem;
    font-size: $section-header-font-size-mobile;
    border-bottom: $section-header-border-width solid #9CCC65;
    display: inline-block;

    @include for-desktop {
      font-size: $section-header-font-size-desktop;
    }
  }

  &__experience-display {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: space-evenly;
    margin: 0 auto;

    &__experience {
      max-width: 400px;
      margin: 0 2rem;
      flex: 1 0 33.33%;
    }
    
    &__wrapper {
      margin: 1.2rem;
    }
  }
}
</style>

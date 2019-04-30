<template>
  <section class="section-experience-dev">
    <div class="section-experience-dev__content">
      <h1 class="section-experience-dev__header">Developer xp</h1>
      <section class="section-experience-dev__experience-display">
        <div class="section-experience-dev__experience-display__wrapper">
          <dev-project
            title="Play with Ninja"
            description="Enter for your chance to game with Ninja or win Ninja branded prizes"
            roles="[role1, role2]"
            class="section-experience-dev__experience-display__experience"
          />
          <button-outlined 
            class="section-experience-dev__experience-display__button"
          />
        </div>
        <div class="section-experience-dev__experience-display__wrapper">
        <dev-project
          title="Small thanks with Google"
          description="Web app where business users can print and download promotional materials"
          class="section-experience-dev__experience-display__experience"
        />
        <button-outlined
          class="section-experience-dev__experience-display__button"
        />
        </div>
      </section>
    </div>
  </section>
</template>
<script>
import DevProject from '../components/project-dev.vue';
import ButtonOutlined from '../components/button-outlined.vue';

export default {
  name: 'section-experience-dev',
  components: {
    DevProject,
    ButtonOutlined
  }
}
</script>
<style lang="scss">
@import '../assets/global-styles.scss';

.section-experience-dev {
  height: $section-height;

  &__header {
    font-size: $section-header-font-size;
    width: $section-header-width;
    margin: 0 auto;
    border-bottom: $section-header-border-width solid #9CCC65;
  }

  &__experience-display {
    display: flex;
    flex-direction: row;
    flex: 0 1 50%;
    width: $section-content-width;
    margin: 0 auto;
    padding-top: $section-content-padding-top;

    &__wrapper {
      max-width: 500px;
      max-height: 300px;
      height: 100%;
      margin: 0 auto;
    }

    &__experience {
      margin: 0 auto;
    }
  }
}
</style>

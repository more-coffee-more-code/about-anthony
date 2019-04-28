<template>
  <section class="section-experience-dev">
    <div class="section-experience-dev__content">
      <h1 class="section-experience-dev__header">Developer xp</h1>
      <section class="section-experience-dev__experience-display">
        <dev-project
          title="Play with Ninja"
          description="Enter for your chance to game with Ninja or win Ninja branded prizes"
          class="section-experience-dev__experience-display__experience"
        />
        <dev-project
          title="Small thanks with Google"
          description="Web app where business users can print and download promotional materials"
          class="section-experience-dev__experience-display__experience"
        />
      </section>
    </div>
  </section>
</template>
<script>
import DevProject from '../components/project-dev.vue';

export default {
  name: 'section-experience-dev',
  components: {
    DevProject
  }
}
</script>
<style lang="scss">
@import '../assets/global-styles.scss';

.section-experience-dev {
  height: $section-height;

  &__header {
    font-size: $section-header-font-size;
    width: 610px;
    margin: 0 auto;
    border-bottom: 4px solid #9CCC65;
  }

  &__experience-display {
    display: flex;
    flex-direction: row;
    flex: 0 1 50%;

    &__experience {
      margin: 0 auto;
    }
  }
}
</style>

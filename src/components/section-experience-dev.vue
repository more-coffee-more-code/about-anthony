<template>
  <section class="section-experience-dev">
    <div class="section-experience-dev__content">
      <h1 class="section-experience-dev__header">Developer xp</h1>
      <section class="section-experience-dev__experience-display">
        <dev-project/>
      </section>
    </div>
  </section>
</template>
<script>
// import DevProject from 'project-dev.vue';
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
  }
}
</style>

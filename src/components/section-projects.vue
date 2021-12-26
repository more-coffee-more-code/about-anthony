<template>
  <div class="section-projects">
    <div class="section-projects__wrapper">
      <h1 class="section-projects__header">Projects</h1>
      <div class="section-projects__cards">
        <project title="Drawing App" description="Create pixelated art by selecting a color and clicking on the canvas." link="https://more-coffee-more-code.github.io/pixel-drawing-app/"/>
        <project title="Blue Ridge Mobile Autocare" description="Designed and developed a PWA for a mobile detailing and autocare company." link="https://blueridgemobileautocare.com/"/>
        <project title="Ars Technica Search" description="App that queries Ars Technica's API and renders the search results." link="https://more-coffee-more-code.github.io/parsely-search/"/>
        <project title="The Purple Cow" description="Users can see the number of total hits received by the Counter API." link="https://more-coffee-more-code.github.io/fearless-trial-project/"/>
      </div>
    </div>
  </div>
</template>
<script>
import Project from '../components/project.vue'

export default {
  name: 'SectionProjects',
  components: {
    Project
  }
}
</script>
<style lang="scss" scoped>
@import '../assets/global-styles.scss';

.section-projects {
  min-height: $section-height;
  padding: 100px 0;

  &__cards {
    display: flex;
    flex-direction: row;
    justify-content: center;
    flex-wrap: wrap;
    max-width: 1200px;
    margin: 0 auto;
    min-height: fit-content;
  }

  &__header {
    font-size: $section-header-font-size-mobile;
    margin: 0 auto 7rem;
    border-bottom: $section-header-border-width solid #9CCC65;
    display: inline-block;

    @include for-desktop {
      font-size: $section-header-font-size-desktop;
    }
  }
}
</style>
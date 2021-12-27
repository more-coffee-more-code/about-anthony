<template>
  <div class="section-projects">
    <div class="section-projects__wrapper">
      <h1 class="section-projects__header">Projects</h1>
      <div class="section-projects__cards">
        <project
          title="Drawing App"
          description="Create pixelated art by selecting a color and clicking on the canvas."
          link="https://more-coffee-more-code.github.io/pixel-drawing-app"
        />
        <project
          title="Blue Ridge Mobile Autocare"
          description="Designed and developed a PWA for a mobile detailing and autocare company."
          link="https://blueridgemobileautocare.com"
        />
        <project
          title="Ars Technica Search"
          description="App that queries Ars Technica's API and renders the search results."
          link="https://more-coffee-more-code.github.io/parsely-search"
        />
        <project
          title="The Purple Cow"
          description="Users can see the number of total hits received by the Counter API."
          link="https://more-coffee-more-code.github.io/fearless-trial-project"
        />
        <project
          title="Adidas Boston Marathon"
          description="Performed Black Box and Exploratory testing."
          link="https://clios.com/sports/winner/direct/adidas-running/here-to-create-legend-58122"
        />
        <project
          title="Think with Google"
          description="Conducted User Acceptance and Exploratory testing."
          link="https://www.thinkwithgoogle.com/feature/mobile-gaming-genres"
        />
        <project
          title="Google Pixel"
          description="Performed Exploratory testing on the retail demo apps for the Pixel 3a and 4a."
        />
        <project
          title="EVMS Virtual Tour"
          description="Virutal tour website built using A-Frame along with 360 degree images and videos."
          link="https://www.evms.edu/virtualtour"
        />
        <project
          title="Lily Center"
          description="Custom WordPress theme developed for Grace College."
          link="https://lakes.grace.edu"
        />
        <project
          title="Marketing Kit with Google"
          description="Robust site that allows businesses to download and print promotional materials."
          link="https://marketingkit.withgoogle.com"
        />
      </div>
    </div>
  </div>
</template>
<script>
import Project from "../components/project.vue";

export default {
  name: "SectionProjects",
  components: {
    Project,
  },
};
</script>
<style lang="scss" scoped>
@import "../assets/global-styles.scss";

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
    border-bottom: $section-header-border-width solid $color-light-green;
    display: inline-block;

    @include for-desktop {
      font-size: $section-header-font-size-desktop;
    }
  }
}
</style>
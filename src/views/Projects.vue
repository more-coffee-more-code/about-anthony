<template>
  <div class="projects">
    <!-- <project title="Drawing App" description="Web app built using Vue.js. Users can create pixelated art by selecting a color and clicking on the canvas." link="https://more-coffee-more-code.github.io/pixel-drawing-app/"/>
    <project title="Blue Ridge Mobile Autocare" description=""/> -->
  </div>
</template>
<script>
export default {
  name: 'Projects'
}
</script>
<style lang="scss" scoped>
@import '../assets/global-styles.scss';

.projects {
  display: flex;
  flex-direction: row;
  justify-content: center;
  flex-wrap: wrap;
  max-width: 1200px;
  margin: 0 auto;
}
</style>
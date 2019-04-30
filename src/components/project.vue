<template>
  <div class="project-dev">
    <h1 class="project-dev__project-title">{{ title }}</h1>
    <p class="project-dev__project-details">{{ description }}</p>
    <!-- <p v-for="role in roles" :key="role" class="project-dev__project-roles"> -->
      <!-- <span class="project-dev__project-roles__role">{{ role }}</span> -->
    <!-- </p> -->
  </div>
</template>
<script>
export default {
  name: 'project-dev',
  props: [
    "title",
    "description",
    // "roles"
  ]
}
</script>
<style lang="scss">
@import '../assets/global-styles.scss';

.project-dev {

  &__project {

    &-title {
      font-size: 2.4rem;  
      color: $color-light-green;
    }
    
    &-details {
      font-size: 1.2rem;
      margin: 0 auto;
      width: 60%;
      font-size: 1.4rem;
    }
  }
}
</style>

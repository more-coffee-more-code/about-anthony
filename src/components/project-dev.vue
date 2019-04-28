<template>
  <div class="project-dev">
    <h1 class="project-dev__project-title">{{ title }}</h1>
    <p class="project-dev__project-details">{{ description }}</p>
  </div>
</template>
<script>
export default {
  name: 'project-dev',
  props: [
    "title",
    "description"
  ]
}
</script>
<style lang="scss">
.project-dev {

  &__project {

    &-title {
      font-size: 1.4rem;  
    }
    
    &-details {
      font-size: 1.2rem;
      margin: 0 auto;
      width: 50%;
    }
  }
}
</style>

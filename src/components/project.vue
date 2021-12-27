<template>
  <div class="project-dev">
    <h1 class="project-dev__project-title">{{ title }}</h1>
    <p class="project-dev__project-details">{{ description }}</p>
    <a  v-if="link" :href="link" target="_blank" class="project-dev__project-link"
      >Go to project &rarr;</a>
    <p v-if="!link" class="project-dev__project-link">No link available</p>
  </div>
</template>
<script>
export default {
  name: "project-dev",
  props: {
    title: String,
    description: String,
    link: String,
  }
};
</script>
<style lang="scss">
@import "../assets/global-styles.scss";

.project-dev {
  border: solid 1px $color-light-green;
  max-width: 300px;
  height: fit-content;
  text-align: left;
  padding: 20px;
  margin: 10px;

  &__project {
    &-title {
      font-size: 1.3rem;
      color: $color-light-green;
    }

    &-details {
      font-size: 1rem;
    }

    &-link {
      color: $color-light-green;
      text-decoration: none;
      cursor: pointer;
      margin: 0;

      &:hover {
        text-decoration: underline;
      }
    }
  }

  &__tech-list {
    list-style: none;
    display: flex;
    flex-direction: row;
    justify-self: flex-end;
    padding-left: 0;
    margin-bottom: 0;

    & li {
      margin-right: 10px;
    }
  }

  &__label {
    margin: 50px 0 0;
  }
}
</style>

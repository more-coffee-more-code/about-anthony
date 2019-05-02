<template>
  <div id="app">
    <loader v-if="isLoading" class="loader"/>
    <router-view v-if="!isLoading"/>
  </div>
</template>
<script>
import Loader from '.././src/components/loader.vue';

export default {
  name: 'app',
  components: {
    Loader
  },
  data() {
    return {
      isLoading: true
    }
  },
  mounted() {
    setTimeout(() => {
      this.isLoading = false;
    }, 2000);
  }
}
</script>
<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #fafafa;
}
#nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}

.loader {
  background-color: black;
  overflow-y:hidden;
}

</style>

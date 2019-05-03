<template>
  <div id="app">
    <loader v-if="isLoading" class="app__loader"/>
    <router-view class="app__home" v-if="!isLoading"/>
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
    }, 200);
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

.app {
  &__loader {
    background-color: black;
    overflow-y:hidden;
    transition: .5s ease-in;
  }

  &__home {
    animation-name: fade-in;
    animation-duration: 0.8s;

    @keyframes fade-in {
      from { opacity: 0; }
      to { opacity: 1}
    }
  }
}
</style>

<template>
  <div id="app">
    <router-view class="app__home" />
  </div>
</template>
<script>
export default {
  name: "app",
};
</script>
<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
  -webkit-tap-highlight-color: transparent;
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
    overflow-y: hidden;
    transition: 0.5s ease-in;
  }

  &__home {
    animation-name: fade-in;
    animation-duration: 0.8s;

    @keyframes fade-in {
      from {
        opacity: 0;
      }
      to {
        opacity: 1;
      }
    }
  }
}
</style>

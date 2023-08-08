<template>
  <main-header v-if="!registerC"></main-header>
  <router-view />
  <main-footer v-if="!registerC"></main-footer>
</template>

<script>
import MainFooter from "./components/layout/MainFooter.vue";
import MainHeader from "./components/layout/MainHeader.vue";
export default {
  components: { MainHeader, MainFooter },
  data() {
    return {
      registers: ["register"],
    };
  },
  computed: {
    registerC() {
      return this.registers.includes(this.$route.name);
    },
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>

<template>
  <div id="app">
    <the-header />
    <div id="nav">
      <router-link to="/">Home</router-link>|
      <router-link to="/about">About</router-link>
    </div>
    <router-view />
    <the-footer />
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";
import TheHeader from "@/components/TheHeader.vue";
import TheFooter from "@/components/TheFooter.vue";

@Component({
  components: {
    TheHeader,
    TheFooter
  }
})
export default class App extends Vue {}
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
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

hr {
  width: 8%;
  background-color: #f63954;
}

h1,
h2,
h3,
button,
a {
  text-transform: uppercase;
  font-family: "Open Sans", "Roboto", Arial, Helvetica, sans-serif;
}

h2.subtitle {
  text-transform: capitalize;
}

.subtitle {
  color: #5a5665;
}
</style>

<template>
  <b-navbar>
    <template slot="brand">
      <b-navbar-item tag="router-link" :to="{ path: '/' }">
        <img
          src="https://raw.githubusercontent.com/buefy/buefy/dev/static/img/buefy-logo.png"
          alt="Lightweight UI components for Vue.js based on Bulma"
        />
      </b-navbar-item>
    </template>

    <template slot="start">
      <b-navbar-item tag="router-link" :to="{ path: '/' }">Home</b-navbar-item>
      <b-navbar-item tag="router-link" :to="{ path: '/' }"
        >Join X-Team</b-navbar-item
      >
      <b-navbar-item tag="router-link" :to="{ path: '/' }"
        >Our Developers</b-navbar-item
      >
      <b-navbar-item tag="router-link" :to="{ path: '/' }"
        >Unleash</b-navbar-item
      >
      <b-navbar-item tag="router-link" :to="{ path: '/' }">Blog</b-navbar-item>
      <b-navbar-item tag="router-link" :to="{ path: '/' }"
        >Portfolio</b-navbar-item
      >
    </template>

    <template slot="end">
      <b-navbar-item tag="div">
        <b-button tag="router-link" :to="{ path: '/' }" type="is-danger"
          >Hire X-Team</b-button
        >
      </b-navbar-item>
    </template>
  </b-navbar>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class Header extends Vue {
  // @Prop() private propName!: propType;
}
</script>

<style scoped lang="scss"></style>

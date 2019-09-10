<template>
  <section class="hero is-priamry is-large">
    <div class="hero-body">
      <h1 class="title">
        Keep Moving
        <em>Forward</em>.
      </h1>
      <h2 class="subtitle">
        X-Team provides high-performing, on-demand teams of developers for
        leading brands.
      </h2>
      <b-button type="is-dark" size="is-medium" outlined>Watch Video</b-button>
    </div>
    <div class="hero-foot">
      <slot></slot>
    </div>
  </section>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class Hero extends Vue {}
</script>

<style scoped lang="scss"></style>

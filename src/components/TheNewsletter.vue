<template>
  <section class="section has-background-white-ter">
    <div class="container">
      <h1 class="title">Keep Moving Forward.</h1>
      <h2 class="subtitle">
        Join the 30,000 developers who subscribe to our newsletter.
      </h2>
      <div class="columns">
        <div class="column"></div>
        <div class="column is-half">
          <b-field>
            <b-input
              placeholder="Your e-mail address"
              size="is-medium"
            ></b-input>
          </b-field>
        </div>
        <div class="column">
          <b-button type="is-danger" size="is-medium">Subscribe</b-button>
        </div>
        <div class="column"></div>
      </div>
    </div>
  </section>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class Newsletter extends Vue {}
</script>

<style scoped lang="scss"></style>

<template>
  <div class="column is-half">
    <div class="columns">
      <div class="column is-one-third">
        <figure class="is-pulled-right">
          <slot name="icon"></slot>
        </figure>
      </div>
      <div class="column has-text-left">
        <h1 class="title is-4">
          <slot name="title"></slot>
        </h1>
        <p>
          <slot name="text"></slot>
        </p>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class ContentTextIconItem extends Vue {}
</script>

<style scoped lang="scss">
p {
  margin-top: -1.5em;
  margin-bottom: 5em;
}
</style>

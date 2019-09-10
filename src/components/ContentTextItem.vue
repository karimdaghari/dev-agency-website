<template>
  <section class="section">
    <div class="container">
      <div class="has-text-centered">
        <h1 class="title"><slot name="title"></slot>.</h1>
        <hr style="margin-left: 46%" />
        <h4 class="subtitle">
          <slot name="subtitle"></slot>
        </h4>
      </div>
      <slot name="content"></slot>
    </div>
  </section>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class ContentTextItem extends Vue {}
</script>

<style scoped lang="scss"></style>

<template>
  <section clas="section is-medium">
    <div class="container-fluid">
      <div class="columns is-variable is-4">
        <template v-if="imageDirection === 'left'">
          <div class="column">
            <div class="has-background-white-ter">
              <img
                :src="
                  imageSrc ||
                    'https://x-team.com/images/pics/remote-developers.jpg'
                "
                alt="image here"
                class="pull-left"
              />
            </div>
          </div>
          <div class="column is-two-fifths">
            <div class="content has-text-left">
              <div class="content has-text-left">
                <h1 class="title">
                  <slot name="title"></slot>
                </h1>
                <hr />
                <p>
                  <slot name="content"></slot>
                </p>
              </div>
            </div>
          </div>
        </template>

        <template v-else-if="imageDirection === 'right'">
          <div class="column is-two-fifths" style="padding-left: 3%">
            <div class="content has-text-left">
              <h1 class="title">
                <slot name="title"></slot>
              </h1>
              <hr />
              <p>
                <slot name="content"></slot>
              </p>
            </div>
          </div>
          <div class="column">
            <div class="has-background-white-ter">
              <img
                :src="
                  imageSrc ||
                    'https://x-team.com/images/pics/remote-developers.jpg'
                "
                alt="image here"
                class="pull-right"
              />
            </div>
          </div>
        </template>
      </div>
    </div>
  </section>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class ContentPicture extends Vue {
  @Prop(String) readonly imageDirection!: string;
  @Prop(String) readonly imageSrc!: string;
}
</script>

<style scoped lang="scss">
img.pull-left {
  transform: translate(-15px, -10px);
}

img.pull-right {
  transform: translate(15px, -10px);
}
</style>

<template>
  <div class="home">
    <v-hero></v-hero>
    <v-clients />
    <content-picture-item imageDirection="left">
      <template #title
        >bla</template
      >
      <template #content>
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Minus,
        pariatur. Accusantium ut fuga dolore provident sunt laborum accusamus,
        nisi, nihil blanditiis architecto qui non dicta modi perspiciatis,
        dolorum ullam pariatur.
      </template>
    </content-picture-item>

    <content-picture-item imageDirection="right">
      <template #title
        >blou</template
      >
      <template #content>
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Minus,
        pariatur. Accusantium ut fuga dolore provident sunt laborum accusamus,
        nisi, nihil blanditiis architecto qui non dicta modi perspiciatis,
        dolorum ullam pariatur.
      </template>
    </content-picture-item>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import VHero from "@/components/VHero.vue";
import VClients from "@/components/VClients.vue";
import ContentPictureItem from "@/components/ContentPictureItem.vue";

@Component({
  components: {
    VHero,
    VClients,
    ContentPictureItem
  }
})
export default class Home extends Vue {}
</script>

<template>
  <div class="home">
    <v-hero></v-hero>
    <div class="has-background-white-ter">
      <v-clients />
    </div>
    <content-text-unleash-item />

    <!-- Cavalry section -->
    <content-text-item>
      <template #title
        >We are your cavalry</template
      >
      <template #subtitle>
        Since 2006, the world’s leading brands have turned to X-Team to help
        them scale their development teams.
      </template>
      <template #content>
        <section class="section">
          <div class="columns">
            <!-- Hire devs card  -->
            <div class="column">
              <div class="card">
                <div class="card-image">
                  <figure class="image">
                    <img
                      src="https://x-team.com/images/pics/hire-developers-1.jpg"
                    />
                  </figure>
                </div>
                <div class="card-content">
                  <div class="content">
                    <h1 class="title is-4">Hire developers</h1>
                    <a href="#">Learn More</a>
                  </div>
                </div>
              </div>
            </div>
            <!-- Work for x-team card -->
            <div class="column">
              <div class="card">
                <div class="card-image">
                  <figure class="image">
                    <img src="https://x-team.com/images/pics/join-x-team.jpg" />
                  </figure>
                </div>
                <div class="card-content">
                  <div class="content">
                    <h1 class="title is-4">Work for x-team</h1>
                    <a href="#">Learn More</a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </section>
      </template>
    </content-text-item>

    <content-text-item>
      <template #title
        >Title test</template
      >
      <template #subtitle
        >Subtitle test</template
      >
    </content-text-item>
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
import ContentTextItem from "@/components/ContentTextItem.vue";
import ContentTextUnleashItem from "@/components/ContentTextUnleashItem.vue";

@Component({
  components: {
    VHero,
    VClients,
    ContentPictureItem,
    ContentTextItem,
    ContentTextUnleashItem
  }
})
export default class Home extends Vue {}
</script>

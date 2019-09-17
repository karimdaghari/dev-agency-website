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

    <!-- Our partners section -->
    <content-text-item>
      <template #title
        >Our partner benefits</template
      >
      <template #subtitle
        >We’ve built partnerships with leading brands that have lasted nearly a
        decade thanks to the level of care & attention we provide.</template
      >
      <template #content>
        <div class="columns">
          <div class="column">
            <div class="content">
              <figure class="image is-48x48">
                <img src="https://x-team.com/images/icons/dedicated-team.svg" />
              </figure>
              <h1 class="title is-5">Dedicated Team.</h1>
              <p>A full-time, scaleable team of trusted developers.</p>
            </div>
          </div>
          <div class="column">
            <div class="content">
              <figure class="image is-48x48">
                <img src="https://x-team.com/images/icons/daily-updates.svg" />
              </figure>
              <h1 class="title is-5">Motivated Developers.</h1>
              <p>
                Developers are given perks to help them learn, grow and stay
                healthy.
              </p>
            </div>
          </div>
          <div class="column">
            <div class="content">
              <figure class="image is-48x48">
                <img
                  src="https://x-team.com/images/icons/account-manager.svg"
                />
              </figure>
              <h1 class="title is-5">Account Manager.</h1>
              <p>Dedicated account manager, available any time.</p>
            </div>
          </div>
          <div class="column">
            <div class="content">
              <figure class="image is-48x48">
                <img
                  src="https://x-team.com/images/icons/flexible-contract.svg"
                />
              </figure>
              <h1 class="title is-5">Flexible Contract.</h1>
              <p>Flexible contracts with simple monthly billing.</p>
            </div>
          </div>
        </div>
      </template>
    </content-text-item>

    <!-- The right team section -->
    <content-text-item>
      <template #title
        >the right team</template
      >
      <template #subtitle
        >Below, watch Kaplan Inc., one of the largest education companies in the
        world, explain why they partner with X-Team to build their
        products.</template
      >
      <template #content>
        <p>Vid here</p>
      </template>
    </content-text-item>
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

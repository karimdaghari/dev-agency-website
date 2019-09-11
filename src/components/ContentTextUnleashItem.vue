<template>
  <div>
    <content-text-item>
      <template #title>
        Unleash
        <span class="plus">+</span>
      </template>
      <template #subtitle
        >One of the ultimate perks of being an X-Teamer is your Unleash+
        membership, which gives you $2,500 per year to use toward activities
        that keep you energized so you can learn, grow and unleash your
        potential.</template
      >
      <template #content>
        <div class="columns is-centered is-multiline is-gapless">
          <content-text-icon-item>
            <template #icon>
              <img
                src="https://x-team.com/images/unleash/conference.svg"
                alt="Conference image"
              />
            </template>
            <template #title
              >Conferences</template
            >
            <template #text
              >Get inspired by hearing stories and meeting extraordinary new
              people. Includes flights and accommodation.</template
            >
          </content-text-icon-item>
          <content-text-icon-item>
            <template #icon>
              <img src="https://x-team.com/images/unleash/gym.svg" />
            </template>
            <template #title
              >GYM MEMBERSHIP</template
            >
            <template #text
              >There's no better way to refocus and stabilize your mind than
              through exercise. Grab a gym membership on us.</template
            >
          </content-text-icon-item>
          <content-text-icon-item>
            <template #icon>
              <img src="https://x-team.com/images/unleash/fresh.svg" />
            </template>
            <template #title
              >FRESH PRODUCE</template
            >
            <template #text
              >We unleash best when we're at our healthiest. Examples include:
              farmers market purchases, produce subscription boxes, local
              grocery, etc.</template
            >
          </content-text-icon-item>
          <content-text-icon-item>
            <template #icon>
              <img src="https://x-team.com/images/unleash/books.svg" />
            </template>
            <template #title
              >Books</template
            >
            <template #text
              >Get books or courses of all kinds, from programming to cooking
              and everything in-between, you decide.</template
            >
          </content-text-icon-item>
          <content-text-icon-item>
            <template #icon>
              <img src="https://x-team.com/images/unleash/meditation.svg" />
            </template>
            <template #title
              >HEALTH & WELLNESS</template
            >
            <template #text
              >Anything wellness-related that helps you relax and recharge.
              Examples: massages, therapy sessions, meditation apps,
              etc.</template
            >
          </content-text-icon-item>
          <content-text-icon-item>
            <template #icon>
              <img src="https://x-team.com/images/unleash/productivity.svg" />
            </template>
            <template #title
              >PRODUCTIVITY APPS</template
            >
            <template #text
              >Get any productivity apps that help you stay organized and more
              at ease.</template
            >
          </content-text-icon-item>
          <content-text-icon-item>
            <template #icon>
              <img src="https://x-team.com/images/unleash/games.svg" />
            </template>
            <template #title
              >Games</template
            >
            <template #text
              >Enjoy a new title each month to help you re-energize.</template
            >
          </content-text-icon-item>
          <content-text-icon-item>
            <template #icon>
              <img src="https://x-team.com/images/unleash/course.svg" />
            </template>
            <template #title
              >Courses</template
            >
            <template #text
              >Never stop learning by getting an online or in-person course on
              ANY topic.</template
            >
          </content-text-icon-item>
          <content-text-icon-item>
            <template #icon>
              <img
                class="image is-64x64"
                src="https://x-team.com/images/unleash/photo.svg"
              />
            </template>
            <template #title
              >Photo Equipment</template
            >
            <template #text
              >Get photography accessories and apps to help you capture the
              beauty the world has to offer.</template
            >
          </content-text-icon-item>
          <content-text-icon-item>
            <template #icon>
              <img
                class="image is-64x64"
                src="https://x-team.com/images/unleash/babysitter.svg"
              />
            </template>
            <template #title
              >Babysitter</template
            >
            <template #text
              >Making time for our loved ones is key to our wellbeing. Hire a
              babysitter so you can get out & recharge.</template
            >
          </content-text-icon-item>
        </div>
      </template>
    </content-text-item>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";
import ContentTextItem from "./ContentTextItem.vue";
import ContentTextIconItem from "./ContentTextIconItem.vue";

@Component({
  components: {
    ContentTextItem,
    ContentTextIconItem
  }
})
export default class ContentTextUnleashItem extends Vue {}
</script>

<style scoped lang="scss">
.plus {
  color: #f63954;
  margin-left: -0.3em;
}
</style>

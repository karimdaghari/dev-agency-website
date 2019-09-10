<template>
  <div class="home">
    <VHero></VHero>
    <VClients />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import VClients from "@/components/VClients.vue";
import VHero from "@/components/VHero.vue";

@Component({
  components: {
    VClients,
    VHero
  }
})
export default class Home extends Vue {}
</script>

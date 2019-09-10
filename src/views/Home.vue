<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <p>Hello</p>
    <VClients />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import VClients from "@/components/VClients.vue";

@Component({
  components: {
    VClients
  }
})
export default class Home extends Vue {}
</script>

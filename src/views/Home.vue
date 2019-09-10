<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <p>Hello</p>
    <Clients />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import Clients from "@/components/Clients.vue";

@Component({
  components: {
    Clients
  }
})
export default class Home extends Vue {}
</script>

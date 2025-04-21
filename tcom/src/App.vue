<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Nav from "@/components/Nav.vue";
</script>

<template>
  <Nav></Nav>
  <div class="Roboto text-lg text-gray-800">
    This is Roboto Mono
  </div>

</template>

<style scoped>
  @import url(
  "https://fonts.googleapis.com/css2?family=Roboto+Mono:ital,wght@0,100..700;1,100..700&display=swap"
  );

  .Roboto {
    font-family: 'Roboto Mono', sans-serif;
  }

</style>

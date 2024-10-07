<script setup>
import HomePage from "@/pages/HomePage.vue";
import AboutPage from "@/pages/AboutPage.vue";

import BaseLayout from "@/components/BaseLayout.vue";
import { ref } from "vue";
import BouttonPage from "@/pages/BouttonPage.vue";
import AnswerPage from "@/pages/AnswerPage.vue";


const page = ref("home");

page.value = "home";
</script>

<template>
  <BaseLayout @root="page = $event">
  <HomePage v-if="page === 'home'" />
  <AboutPage v-if="page === 'about'" />
    <BouttonPage v-if="page === 'bouttons'" />
    <AnswerPage v-if="page === 'answer'" />
  </BaseLayout>

</template>

<style scoped>

</style>
<script setup>
import HomePage from "@/pages/HomePage.vue";
import BaseHeader from "@/components/BaseHeader.vue";
import BaseFooter from "@/components/BaseFooter.vue";

</script>

<template>
  <BaseHeader />
  <main><HomePage /></main>

  <BaseFooter />

</template>

<style scoped>
main{
  margin-top: 10%;
}
</style>
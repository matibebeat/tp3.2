<script setup>

import BaseFooter from "@/components/BaseFooter.vue";
import BaseHeader from "@/components/BaseHeader.vue";
</script>

<template>
  <BaseHeader />
  <main><slot></slot></main>

  <BaseFooter />
</template>

<style scoped>
main{
  margin-top: 10%;
}

</style>
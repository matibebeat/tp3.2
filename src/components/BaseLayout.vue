<script setup>

import BaseFooter from "@/components/BaseFooter.vue";
import BaseHeader from "@/components/BaseHeader.vue";
</script>

<template>
  <BaseHeader @root="$emit('root', $event)"/>
  <main><slot></slot></main>

  <BaseFooter />
</template>

<style scoped>
main{
  margin-top: 10%;
  margin-left: 320px;
  margin-right: 320px;
  margin-bottom: 10%;
}

</style>
<script setup>
import {ref} from "vue";
import BaseButton from "@/components/BaseButton.vue";
import AsyncButton from "@/components/AsyncButton.vue";

const direBonjour = () => {
  return new Promise((resolve) => {
    setTimeout(() => {
      console.log("Bonjour");
      resolve();
    }, 1000);
  });
};
</script>

<template>
  <h1>Home page</h1>
  <div>

    <BaseButton size="large" color="primary" type="normal">Subscribe</BaseButton>
    <BaseButton size="large" color="secondary" type="normal">Like</BaseButton>
    <BaseButton size="large " color="primary" type="disabled">Unsubscribe</BaseButton>

  </div>

  <AsyncButton size="small" color="danger" :funct="direBonjour">Click me</AsyncButton>
</template>

<style scoped>
div{
  display: flex;
  gap: 20px;
  margin-top: 20px;
}
*{
  margin-bottom: 25px;
}
</style>
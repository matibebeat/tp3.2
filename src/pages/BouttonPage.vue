<script setup>

import BaseButton from "@/components/BaseButton.vue";
</script>

<template>
  <h1>Boutton</h1>
  <p>Here are all the possibles buttons</p>

  <h2>Primary</h2>
  <div class="wrapper">
    <BaseButton size="large" color="primary" type="normal">Boutton</BaseButton>
    <BaseButton size="medium" color="primary" type="normal">Subscribe</BaseButton>
    <BaseButton size="small" color="primary" type="normal">Subscribe</BaseButton>
  </div>

  <h3>disabled</h3>
  <div class="wrapper">
    <BaseButton size="large" color="primary" type="disabled">Unsubscribe</BaseButton>
    <BaseButton size="medium" color="primary" type="disabled">Unsubscribe</BaseButton>
    <BaseButton size="small" color="primary" type="disabled">Unsubscribe</BaseButton>
  </div>


  <h2>Secondary</h2>
  <div class="wrapper">
    <BaseButton size="large" color="secondary" type="normal">Like</BaseButton>
    <BaseButton size="medium" color="secondary" type="normal">Like</BaseButton>
    <BaseButton size="small" color="secondary" type="normal">Like</BaseButton>
  </div>

  <h3>disabled</h3>
  <div class="wrapper">
    <BaseButton size="large" color="secondary" type="disabled">Unsubscribe</BaseButton>
    <BaseButton size="medium" color="secondary" type="disabled">Unsubscribe</BaseButton>
    <BaseButton size="small" color="secondary" type="disabled">Unsubscribe</BaseButton>
  </div>


  <h2>Warning</h2>
  <div class="wrapper">
    <BaseButton size="large" color="warning" type="normal">Attention à vous</BaseButton>
    <BaseButton size="medium" color="warning" type="normal">Attention à vous</BaseButton>
    <BaseButton size="small" color="warning" type="normal">Attention à vous</BaseButton>
  </div>


  <h2>Danger</h2>
  <div class="wrapper">
    <BaseButton size="large" color="danger" type="normal">Attention à vous</BaseButton>
    <BaseButton size="medium" color="danger" type="normal">Attention à vous</BaseButton>
    <BaseButton size="small" color="danger" type="normal">Attention à vous</BaseButton>
  </div>

</template>

<style scoped>
.wrapper{
  display: flex;
  gap: 20px;
  margin-top: 20px;
}

</style>
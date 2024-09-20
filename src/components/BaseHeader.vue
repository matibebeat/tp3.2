<script setup>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import BaseButton from "@/components/BaseButton.vue";
</script>

<template>
  <header>
    <h1>TP 3.2</h1>
    <nav>
      <BaseButton
        color="primary"
        size="small"
        type="enabled"
      >Home</BaseButton>
      <BaseButton
          color="primary"
        size="small"
        type="enabled"

      >About</BaseButton>
    </nav>
    <div>
      <BaseButton
        color="danger"
        size="small"
        type="enabled">Leave</BaseButton>

    </div>


  </header>
</template>

<style scoped>
  header {
    background-color: rgba(68, 59, 59, 0.2);
    backdrop-filter: blur(10px);
    border-radius: 18px;
    color: #white;
    padding: 10px 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    top: 1%;
    position: fixed;
    left: 5%;
    right: 5%;
    border: 1px solid rgba(68, 59, 59, 0.3);
  }
  a {
    color: white;
    margin-right: 10px;
  }

  h1{
    margin: 0;
  }

  nav {
    display: flex;
    gap: 50px;
  }

</style>
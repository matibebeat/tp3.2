<script setup>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import BaseButton from "@/components/BaseButton.vue";

import { ref } from "vue";

const active = ref("home");
</script>

<template>
  <header>
    <div class="top">


    <h1>myTP 3.2</h1>

    <div class="profile">
      <p>Mathis LAIR</p>
      <img src="https://media.licdn.com/dms/image/v2/C4E03AQFb3VLzy61s6g/profile-displayphoto-shrink_200_200/profile-displayphoto-shrink_200_200/0/1633769494020?e=2147483647&v=beta&t=Or9aW_ffsCgKBq8u4XXo4pNP2qNy5zZzCNKxiyPu8fw" alt="avatar" />

    </div>
    </div>
    <nav>
      <a href="#" :class="active === 'home'? 'active': '' " @click="$emit('root', 'home'); active = 'home'">HOME</a>
      <a href="#" :class="active === 'about'? 'active': '' " @click="$emit('root', 'about'); active = 'about'">ABOUT</a>
      <a href="#" :class="active === 'bouttons'? 'active': '' " @click="$emit('root', 'bouttons'); active = 'bouttons'">BOUTTONS</a>
      <a href="#" :class="active === 'answer'? 'active': '' " @click="$emit('root', 'answer'); active = 'answer'">ANSWER</a>
    </nav>
  </header>
</template>

<style scoped>
  header {
    display: flex;
    flex-direction: column;
    color: White;
    background-color: white;
    justify-content: space-between;
    align-items: center;
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    border-bottom: 1px solid rgb(224, 224, 224);
    z-index: 1;
  }
  .top {
    background-color: rgb(22, 55, 103);
    width: 95%;
    padding:8px 50px;
    display: flex;
    justify-content: space-between;
    align-items: center;

  }
  a {
    color: rgb(97,97,97);
    padding: 12px 12px;
    text-decoration: none;
    font-size: 1.0em;
  }

  a:hover{
    background-color: #d3d3d3;
  }

  .active{
    color: #E7873B;
    border-bottom: 3px solid #E7873B;
  }

  h1{
    margin: 0;
  }

  nav {
    display: flex;
    background-color: white;
    width: 100%;
    justify-content: center;
  }
  .profile{
    display: flex;
    gap: 12px;
    align-items: center;
  }

  img {
    width: 40px;
    height: 40px;
    border-radius: 50%;
  }

  h1{
      font-family: "Sofadi One", system-ui;
      font-weight: 400;
      font-style: normal;

  }
</style>
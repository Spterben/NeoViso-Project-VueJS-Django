<script setup>
import { info } from 'autoprefixer'
import { ref } from 'vue'
import Header from './components/Header.vue'
import AddEvent from './components/AddEvent.vue'
import CardList from './components/CardList.vue'
import Card from './components/Card.vue'
import Register from './components/Register.vue'
import Profile from './components/Profile.vue'
</script>

<template>
  <div>
    <div class="bg-white w-4/5 m-auto rounded-xl shadow-2xl mt-12">
      <Profile />
      <Header />
      <CardList />
      <CardList />
      <CardList />
    </div>
  </div>
</template>

<style scoped></style>

<script setup>
import Card from './Card.vue'
</script>

<template>
  <div>
    <p>{{ categoryName }}</p>
    <div class="whitespace-nowrap overflow-x-auto">
      <Card image-url="/src/components/pictures/like2.png" :isLiked="false" />
      <Card />
      <Card />
    </div>
  </div>
</template>

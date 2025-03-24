<script setup>
import { h } from 'vue'
import Header from './Header.vue'
</script>

<template>
  <div>
    <div class="fixed inset-0 bg-black opacity-60"></div>

    <div class="fixed inset-0 flex justify-center">
      <div class="bg-white w-4/5 m-10 h-auto rounded-3xl">
        <button class="flex p-2 gap-2">
          <img src="/src/components/pictures/profile.png" alt="Cart" class="size-6" />
          <b>Профиль</b>
        </button>
        <div class="flex">
          <button>
            <h1 class="right-0">На главную</h1>
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'
defineProps({
  imageUrl: String,
  isLiked: Boolean,
  onClickLike: Function,
})

const event = ref({
  name: 'Название мероприятия',
  banner: '/src/components/pictures/like2.png',
  info: 'краткая информация о мероприятии',
  likeCount: 0,
  isLike: false,
})

function addLike() {
  if (event.value.isLike) {
    event.value.likeCount--
  } else {
    event.value.likeCount++
  }
  event.value.isLike = !event.value.isLike
}
</script>

<template>
  <div class="inline-block">
    <h1 class="mx-10 my-2">{{ eventCategory }}</h1>
    <div
      class="mx-2 inline-block bg-white border border-slate-100 rounded-3xl p-4 transition hover:-translate-y-2 hover:shadow-xl"
    >
      <button class="cursor-pointer">
        <img :src="imageUrl" alt="Event" class="size-40" />
        <p1 class="">{{ event.name }}</p1>
        <p>{{ event.info }}</p>
      </button>
      <button @click="addLike" class="cursor-pointer flex mt-5 items-center">
        <img
          :src="
            !isLiked ? '/src/components/pictures/like2.png' : '/src/components/pictures/like1.png'
          "
          alt="Like 1"
          class="size-5"
        />
        <p>{{ event.likeCount }}</p>
      </button>
    </div>
  </div>
</template>

<style></style>

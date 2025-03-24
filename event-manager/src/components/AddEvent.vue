<script>
export default {
  data() {
    return {
      organisation: '',
      email: '',
      phoneNumber: '',
      eventName: '',
      banner: '',
      info: '',
      events: [],
    }
  },
  methods: {
    processingData() {
      this.events.push({
        organisator: this.organisator,
        email: this.email,
        phoneNumber: this.phoneNumber,
        eventName: this.eventName,
        banner: this.banner,
        info: this.info,
      })
      this.clearData()
    },
    clearData() {
      this.organisator = ''
      this.email = ''
      this.phoneNumber = ''
      this.eventName = ''
      this.banner = ''
      this.info = ''
    },
  },
}
</script>

<template>
  <div class="flex flex-col">
    <input type="text" v-model="organisator" placeholder="Организатор" />
    <input type="text" v-model="email" placeholder="Email" />
    <input type="number" v-model="phoneNumber" placeholder="Номер телефона" />
    <input type="text" v-model="eventName" placeholder="Название события" />
    <input type="imageUrl" v-model="banner" placeholder="Ссылка на банер мероприятия" />
    <input type="text" v-model="info" placeholder="Информация о событии" />
    <p className="error">{{ errors }}</p>
    <button @click="processingData()">Send</button>

    <p>{{ events }}</p>
  </div>
</template>

<style></style>

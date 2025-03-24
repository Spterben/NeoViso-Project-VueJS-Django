<script>
export default {
  data() {
    return {
      organisation: '',
      email: '',
      phoneNumber: '',
      fioOrganizer: '',
    }
  },
}
</script>

<template>
  <div>
    <div class="fixed inset-0 bg-black opacity-60"></div>

    <div class="fixed inset-0 flex justify-center">
      <div class="bg-white w-4/5 m-10 h-auto px-10 py-5 rounded-3xl">
        <div class="flex">
          <div
            class="flex rounded-xl mx-2 bg-sky-100 cursor-pointer text-slate-400 hover:text-black hover:bg-sky-200 inset-0 justify-center w-1/2"
          >
            <button class="cursor-pointer">User</button>
          </div>
          <div
            class="flex rounded-xl mx-2 bg-sky-100 cursor-pointer text-slate-400 hover:text-black hover:bg-sky-200 right-0 justify-center w-1/2"
          >
            <button class="cursor-pointer">Organisator</button>
          </div>
        </div>
        <div class="flex flex-col my-15 m-auto text-slate-500 px-20 w-3/5">
          <input type="text" v-model="organisatin" placeholder="Организация" />
          <input type="text" v-model="email" placeholder="Email" />
          <input type="value" v-model="phoneNumber" placeholder="Номер телефона" />
          <input type="text" v-model="fioOrganizer" placeholder="ФИО ответственного лица" />
        </div>
      </div>
    </div>
  </div>
</template>

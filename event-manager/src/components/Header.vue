<template>
  <header class="flex justify-between border-b-2 border-purple-100 px-8 py-2">
    <div class="flex items-center gap-1">
      <img src="/src/components/pictures/logo.png" alt="Logo" class="size-14" />
      <div>
        <b class="text-sl uppercase">Every Day Event</b>
        <p class="text-xs text-slate-500">создание и просмотр мероприятий</p>
      </div>
    </div>

    <ul class="flex items-center gap-6">
      <!-- <li>
            <button class="flex items-center gap-1">
              <img src="/src/components/pictures/plus.png" alt="Cart" class="size-6" />
              <b class="text-sm/[100%]">
                Создать <br />
                событие
              </b>
            </button>
          </li> -->

      <li>
        <button class="flex items-center gap-1 cursor-pointer text-slate-600 hover:text-black">
          <img src="/src/components/pictures/like1.png" alt="Cart" class="size-6" />
          <b>Закладки</b>
        </button>
      </li>

      <li>
        <button class="flex items-center gap-1 cursor-pointer text-slate-600 hover:text-black">
          <img src="/src/components/pictures/profile.png" alt="Cart" class="size-6" />
          <b>Профиль</b>
        </button>
      </li>
    </ul>
  </header>
</template>

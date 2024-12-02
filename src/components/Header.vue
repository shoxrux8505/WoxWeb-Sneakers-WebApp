<script setup>
defineProps({
  totalPrice: Number
})

const emit = defineEmits(['openDrawer'])
</script>

<template>
  <header class="flex justify-between border-b border-slate-200 px-10 py-8 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4">
    <router-link to="/">
      <div class="flex items-center gap-4">
        <img src="/logo.png" alt="Logo" class="w-20" />
        <div>
          <h2 class="text-xl font-bold uppercase text-sm md:text-lg lg:text-xl">WoxWeb Sneakers</h2>
          <!-- <p class="text-slate-500">customize sneakers shop</p> -->
        </div>

      </div>
    </router-link>
    <!-- <h1>Boshqacha <span>bo'l</span></h1> -->
    <ul class="flex items-center gap-10">
      <li @click="() => emit('openDrawer')"
        class="flex items-center cursor-pointer gap-3 text-gray-500 hover:text-black">
        <img src="/cart.svg" alt="Cart" />
        <b class="text-sm md:text-lg lg:text-xl">{{ totalPrice }} сум.</b>
      </li>

      <router-link to="/favorites">
        <li class="flex items-center cursor-pointer gap-3 text-gray-500 hover:text-black">
          <img src="/heart.svg" alt="Cart" />
          <span>Закладки</span>
        </li>
      </router-link>

      <!-- <li class="flex items-center cursor-pointer gap-3 text-gray-500 hover:text-black">
        <img src="/profile.svg" alt="Cart" />
        <span>Профиль</span>
      </li> -->
    </ul>
  </header>
</template>

<style>
h1 {
  font-size: 40px;
  font-family: "Playwrite CU", cursive;
  font-optical-sizing: auto;
  font-weight: weight;
  font-style: normal;
}
h1 span{
  color: royalblue;
}
</style>
<template>
  <div class="flex justify-between mx-12 lg:mx-24 py-5">
    <div class="flex">
      <button>
        <img src="../assets/LogoGITS.png" alt="Logo" />
      </button>
      <div class="gap-x-3 lg:flex ml-10 items-center hidden">
        <button class="flex">Home</button>
        <button class="flex">Products<span class="material-symbols-outlined">expand_more</span></button>
        <button class="flex">Categories<span class="material-symbols-outlined">expand_more</span></button>
      </div>
    </div>

    <button class="lg:hidden" @click="toggleMobileMenu">
      <span class="material-symbols-outlined">
        menu
      </span>
    </button>

    <div class="lg:hidden mt-3" :class="{ 'absolute right-10 top-12 bg-[#ffffff] p-3 rounded-lg': isMobileMenuOpen, 'hidden': !isMobileMenuOpen }">
      <button class="block mb-2">Home</button>
      <button class="mb-2 flex">Products<span class="material-symbols-outlined">expand_more</span></button>
      <button class="flex mb-2">Categories<span class="material-symbols-outlined">expand_more</span></button>
      <button class="block mb-2">Log in</button>
      <button class="block mb-2">Sign up</button>
    </div>

    <div class="hidden lg:flex gap-x-3">
      <button class="">Log in</button>
      <button class="bg-[#0984DD] px-[18px] py-[10px] rounded-lg text-white">Sign up</button>
    </div>
  </div>
</template>
  

<script setup lang="ts">
import { ref } from 'vue';

const isMobileMenuOpen = ref(false);

const toggleMobileMenu = () => {
  isMobileMenuOpen.value = !isMobileMenuOpen.value;
};
</script>

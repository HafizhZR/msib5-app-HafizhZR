<template>
  <div class="mb-10">
    <div class="px-10">
      <div class="flex justify-between">
        <p class="font-semibold text-2xl m-14">
          Categories
        </p>
        <button class="text-[#0984DD] flex justify-center items-center gap-3 m-14">
          View all
          <img src="../../../assets/Arrow.png" alt="">
        </button>
      </div>
    </div>
    <div class="grid mx-24 md:grid-cols-3 lg:gap-0 lg:flex justify-center lg:justify-around  lg:mx-24">
      <Card v-for="(kategori, index) in categories" :key="index" :imageUrl="kategori.imageUrl" :name="kategori.name" />
    </div>
  </div>
</template>
  
<script setup lang="ts">
import { ref } from 'vue';
import MensFashion from '../../../assets/MensFashion.png';
import WomensFashion from '../../../assets/WomensFashion.png';
import Bicycle from '../../../assets/Bicycle.png'
import Handphone from '../../../assets/Handphone.png'
import HobbiesAndCollections from '../../../assets/Hobbies&Collections.png'
import HouseHold from '../../../assets/HouseHold.png'
import Card from './Card.vue';


const categories = ref([
  {
    name: `Men's Fashion`,
    imageUrl: MensFashion,
  },
  {
    name: `Women's Fashion`,
    imageUrl: WomensFashion,
  },
  {
    name: 'Bicycle',
    imageUrl: Bicycle,
  },
  {
    name: 'Handphone',
    imageUrl: Handphone,
  },
  {
    name: 'Hobbies and Collections',
    imageUrl: HobbiesAndCollections,
  },
  {
    name: 'Household',
    imageUrl: HouseHold,
  },
]);
</script>
  
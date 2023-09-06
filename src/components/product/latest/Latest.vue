<template>
  <div class="flex flex-col mx-auto">
    <div class="">
      <div class="px-10">
        <div class="flex justify-between w-full">
          <div class="flex justify-center items-center">
            <p class="font-semibold text-2xl ml-14 mr-4">
              Latest Product
            </p>
          </div>
          <button class="text-[#0984DD] flex justify-center items-center gap-3 m-14 ">
            View all
            <img src="../../../assets/Arrow.png" alt="">
          </button>
        </div>
      </div>
      <div class="flex flex-col lg:flex-row justify-center items-center lg:flex gap-6 lg:justify-center lg:items-center lg:ml-50">
        <div class="mb-10 bg-[#28A0F6] w-[352px] h-[494px] p-10 rounded-lg left-10">
          <div class="flex-col mb-20">
            <p class="text-2xl text-white">
              Discount
            </p>
            <p class="text-5xl font-semibold text-white w-1/2">
              More and More
            </p>
          </div>
          <div class="flex-col">
            <p class="text-2xl text-white">
              up To
            </p>
            <p class="text-7xl font-semibold text-[#FCE834]">
              50%
            </p>
          </div>
        </div>
        <div class="lg:z-[1] lg:mt-[-15px] lg:flex flex flex-col lg:flex-row justify-center items-center gap-0 lg:gap-7 lg:ml-[-130px]">
          <Card class="mb-7" v-for="(data, index) in latest" :key="index" :imageUrl="data.imageUrl" :label="data.label"
            :judul="data.judul" :harga="data.harga" :hargaAsli="data.hargaAsli" :diskon="data.diskon" />
        </div>
      </div>
    </div>

  </div>
</template>

<script setup lang="ts">
import Card from '../../Card.vue';
import { ref } from 'vue'
import Bottle from '../../../assets/Bottle.png'

const latest = ref([
  {
    imageUrl: Bottle,
    label: 'Label',
    judul: 'UX review presentations',
    harga: 36000,
    hargaAsli: 40000,
    diskon: 10,
  },
  {
    imageUrl: Bottle,
    label: 'Label',
    judul: 'UX review presentations',
    harga: 36000,
    hargaAsli: 40000,
    diskon: 10,
  },
  {
    imageUrl: Bottle,
    label: 'Label',
    judul: 'UX review presentations',
    harga: 36000,
    hargaAsli: 40000,
    diskon: 10,
  },
  {
    imageUrl: Bottle,
    label: 'Label',
    judul: 'UX review presentations',
    harga: 36000,
    hargaAsli: 40000,
    diskon: 10,
  },

])
</script>
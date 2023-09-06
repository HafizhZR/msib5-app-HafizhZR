<template>
  <div>
    <div class="px-10">
      <div class="flex justify-between ">
        <div class="flex justify-center items-center">
          <p class="font-semibold text-2xl ml-14 mr-4">
            Flash Sale
          </p>
          <p class="bg-[#F04438] h-[30px] px-2 py-2 text-center items-center flex rounded-lg text-white">
            00:12:12
          </p>
        </div>
        <button class="text-[#0984DD] flex justify-center items-center gap-3 m-14 ">
          View all
          <img src="../../../assets/Arrow.png" alt="">
        </button>
      </div>
    </div>
    <div class="md:flex md:justify-around mx-32">
      <Card class="mb-8" v-for="(data, index) in flashSale" :key="index" :imageUrl="data.imageUrl" :label="data.label"
        :judul="data.judul" :harga="data.harga" :hargaAsli="data.hargaAsli" :diskon="data.diskon" />
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';
import Card from '../../../components/Card.vue'
import Bottle from '../../../assets/Bottle.png'
import Sepatu from '../../../assets/Sepatu.png'

const flashSale = ref([
  {
    imageUrl: Bottle,
    label: 'Label',
    judul: 'UX review presentations',
    harga: 36000,
    hargaAsli: 40000,
    diskon: 10,
  },
  {
    imageUrl: Sepatu,
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
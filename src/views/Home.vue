<template>
    <div>
      <div class="bg-gradient-to-b from-[#D8EEFD] to-white w-full">
        <Header />
        <Jumbotron />
      </div>
      <div>
        <Categories />
        <FlashSale />
        <Latest />
        <Promo />
        <Latest />
        <Latest />
        <ForYou />
        <NewsLetter />
      </div>
      <div>
        <Footer />
      </div>
    </div>
  </template>
  
  <script setup lang="ts">
  import Header from '../components/Header.vue'
  import Jumbotron from '../components/home/Jumbotron.vue'
  import Categories from '../components/home/Categories.vue'
  import FlashSale from '../components/home/FlashSale.vue'
  import Latest from '../components/home/Latest.vue'
  import Promo from '../components/home/Promo.vue'
  import ForYou from '../components/home/ForYou.vue'
  import NewsLetter from '../components/NewsLetter.vue'
  import Footer from '../components/Footer.vue'
  </script>
  
<template>
  <div class="bg-gradient-to-b from-sky-200 to-white">
    <div>
      <Header />
    </div>
    <div>
      <Jumbotron />
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
import Header from './components/Header.vue'
import Jumbotron from './components/Jumbotron.vue'
import Categories from './components/product/categories/Categories.vue'
import FlashSale from './components/product/flash-sale/FlashSale.vue'
import Latest from './components/product/latest/Latest.vue'
import Promo from './components/product/promo/Promo.vue'
import ForYou from './components/product/for-you/ForYou.vue'
import NewsLetter from './components/NewsLetter.vue'
import Footer from './components/Footer.vue'

</script>

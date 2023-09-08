<template>
  <div>
    <ViewAll :kategori="Promo" />
    <div class="flex justify-center items-center">
      <div class="w-[83%] h-[200px] bg-slate-200 mx-auto mb-10 rounded-lg">
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
import ViewAll from '../../content/ViewAll.vue'

const Promo = 'Promo'

</script>
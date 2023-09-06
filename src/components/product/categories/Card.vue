<template>
  <div class="flex-col box-border">
    <button class="w-40 h-40">
      <img :src="imageUrl" alt="Gambar" class="mx-auto flex">
      <h6 class="mt-2 text-center">{{ name }}</h6>
    </button>
  </div>
</template>
  
<script setup lang="ts">

const { imageUrl, name } = defineProps({
  imageUrl: String,
  name: String
});

</script>
  
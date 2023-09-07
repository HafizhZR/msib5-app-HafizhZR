<template>
  <button>
    <div class="flex-col mx-auto box-border w-[224px] h-[430px] shadow-lg bg-white rounded-lg">
      <img :src="imageUrl" alt="gambar" class="bg-[#F2F4F7] w-full rounded-lg">
      <div>
        <div class="m-6">
          <p class="px-2 py-1 rounded-2xl bg-[#F2F4F7] w-fit mb-4">
            {{ label }}
          </p>
          <div>
            <h3 class="text-base mb-2 w-5/6 text-left">
              {{ judul }}
            </h3>
            <div class="flex justify-between items-center">
              <p class="font-bold">
                Rp{{ harga }}
              </p>
              <p class="text-xs opacity-50">
                450ML
              </p>
            </div>
            <div class="flex gap-5">
              <p class="text-xs line-through opacity-50">
                Rp{{ hargaAsli }}
              </p>
              <p class="text-xs text-[#B42318] bg-[#fff2f1] rounded-lg px-1">
                -{{ diskon }}%
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </button>
</template>

<script setup lang="ts">

const { imageUrl, label, judul, harga, hargaAsli, diskon } = defineProps({
  imageUrl: String,
  label: String,
  judul: String,
  harga: Number,
  hargaAsli: Number,
  diskon: Number,
})

</script>
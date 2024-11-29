<script setup>
defineProps({
  text: String,
})
</script>

<template>
  <div class="bg-gray-800 w-1/4 min-h-32 rounded-lg">
    <div class="w-full h-full flex flex-col items-center justify-center">
      <div class="rounded-full border border-purple-600 w-14 h-14 p-2 hover:scale-105">
        <div class="w-full h-full rounded-full border border-purple-600"></div>
      </div>
      <p class="text-white">{{ text }}</p>
    </div>
  </div>
</template>
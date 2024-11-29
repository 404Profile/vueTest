<script setup>
defineProps({
  isActive: {
    Boolean,
    default: false,
  },
  text: String,
})
</script>

<template>
  <div>
    <button :class="isActive ? 'border border-gray-700 bg-gray-900 px-3 py-2 rounded-lg' : 'px-3 py-2 hover:bg-gray-900 rounded-lg border border-transparent hover:border-gray-700 transition delay-100 duration-500 ease-in-out'">
      <span class="text-white">{{ text }}</span>
    </button>
  </div>
</template>
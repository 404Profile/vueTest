<script setup>
import {RouterLink} from "vue-router";

defineProps({
  text: String,
});
</script>

<template>
  <div>
    <RouterLink to="#" class="hover:underline hover:scale-105 transition delay-100 duration-300 ease-in-out">
      {{ text }}
    </RouterLink>
  </div>
</template>
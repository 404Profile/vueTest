<script setup>
import HeaderButton from "@/components/HeaderButton.vue";
</script>

<template>
  <header class="flex bg-slate-800 border-b border-gray-700">
    <div class="w-full px-1 sm:px-5 md:px-10">
      <div class="flex justify-between max-w-7xl mx-auto items-center min-h-16">
        <div>
          <RouterLink to="#" class="text-xl font-bold text-white">
            LOGO
          </RouterLink>
        </div>
        <div class="flex space-x-10">
          <header-button is-active="true" text="Home" />
          <header-button text="About Us" />
          <header-button text="Properties" />
          <header-button text="Services" />
          <header-button text="Contact Us" />
        </div>
      </div>
    </div>
  </header>
</template>
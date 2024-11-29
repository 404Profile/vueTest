<script setup>
import {ref} from "vue";
import Modal from "@/components/Modal.vue";

defineProps({
  title: String,
  body: String,
  price: String,
})

const isOpenModal = ref(false);

const openModal = () => {
  isOpenModal.value = true;
  document.body.style.overflow = 'hidden';
}

const closeModal = () => {
  isOpenModal.value = false;
  document.body.style.overflow = null;
}
</script>

<template>
  <article class="w-full">
    <div class="p-4 border border-gray-700 rounded-lg">
      <div class="bg-gray-500 w-full h-96 rounded-lg"></div>

      <div>
        <div>
          <h3 class="text-white text-2xl font-medium">
            {{ title }}
          </h3>

          <p class="pt-2">
            {{ body }}
          </p>
        </div>

        <div class="flex justify-between items-center pt-2">
          <div>
            <p>Price</p>
            <p class="text-white text-2xl font-medium">{{ price }}</p>
          </div>

          <div>
            <button @click="openModal" class="border border-gray-700 bg-indigo-800 px-4 py-3 rounded-lg hover:scale-105 hover:bg-indigo-900">
              <span class="text-white">View Property Details</span>
            </button>
          </div>
        </div>
      </div>
    </div>
  </article>

  <modal @closeModal="closeModal" v-if="isOpenModal" :title="title" :body="body" :price="price"/>

</template>
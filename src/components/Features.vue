<template>
  <div class="block">
    <div class="flex-row space-y-4 sm:mx-0 mx-4 sm:flex sm:space-x-5 sm:space-y-0 mt-20 w-full">
      <div v-for="(card, index) in paginatedFeatures" :key="index">
        <feature-card :title="card.title" :body="card.body" :price="card.price" />
      </div>
    </div>

    <div class="flex justify-center">
      <div class="pagination">
        <button @click="previousPage" :disabled="currentPage === 0">Previous</button>
        <button @click="nextPage" :disabled="currentPage === totalPages - 1">Next</button>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref, computed } from 'vue';
import FeatureCard from "@/components/FeatureCard.vue";

const features = [
  {title: "Seaside Serenity Villa 1", body: "A stunning 4-bedroom, 3-bathroom villa in a peaceful suburban neighborhood…", price: "550"},
  {title: "Seaside Serenity Villa 2", body: "A stunning 4-bedroom, 3-bathroom villa in a peaceful suburban neighborhood…", price: "650"},
  {title: "Seaside Serenity Villa 3", body: "A stunning 4-bedroom, 3-bathroom villa in a peaceful suburban neighborhood…", price: "750"},
  {title: "Feature Card 4", body: "Description for Feature Card 4", price: "800"},
  {title: "Feature Card 5", body: "Description for Feature Card 5", price: "900"},
  {title: "Feature Card 6", body: "Description for Feature Card 6", price: "1000"},
  {title: "Feature Card 7", body: "Description for Feature Card 6", price: "1000"},
  {title: "Feature Card 8", body: "Description for Feature Card 6", price: "1000"},
  {title: "Feature Card 9", body: "Description for Feature Card 6", price: "1000"},
];

const itemsPerPage = 3;
const currentPage = ref(0);

const totalPages = Math.ceil(features.length / itemsPerPage);

const paginatedFeatures = computed(() => {
  const startIndex = currentPage.value * itemsPerPage;
  return features.slice(startIndex, startIndex + itemsPerPage);
});

const nextPage = () => {
  if (currentPage.value < totalPages - 1) {
    currentPage.value++;
  }
};

const previousPage = () => {
  if (currentPage.value > 0) {
    currentPage.value--;
  }
};
</script>

<style>
.pagination {
  margin-top: 10px;
}

button {
  padding: 5px 10px;
  margin-right: 5px;
  cursor: pointer;
}

button:disabled {
  opacity: 0.5;
  cursor: not-allowed;
}
</style>
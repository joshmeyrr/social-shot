<template>
  <main class="flex flex-col gap-2 justify-center">
    <div
      v-for="(card, index) in cards"
      :key="index"
      class="bg-gray-700 w-72 p-8 rounded"
    >
      <h2 class="text-4xl uppercase font-black">
        {{ card.title }}
        <span class="text-orange-400 font-black">#{{ index }}</span>
      </h2>
      <p>
        {{ card.description }}
      </p>
    </div>
  </main>
</template>

<script setup lang="ts">
import { ref } from "vue";

const cards = ref([
  {
    title: "Card",
    description:
      "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Odit, eveniet cumque. Consequatur natus dolorum laboriosam at saepe reprehenderit molestiae, officiis animi, quibusdam fuga corporis laborum!",
  },
  {
    title: "Employee",
    description:
      "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Odit, eveniet cumque. Consequatur natus dolorum laboriosam at saepe reprehenderit molestiae, officiis animi, quibusdam fuga corporis laborum!",
  },
  {
    title: "Customer",
    description:
      "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Odit, eveniet cumque. Consequatur natus dolorum laboriosam at saepe reprehenderit molestiae, officiis animi, quibusdam fuga corporis laborum!",
  },
]);
</script>

<template>
  <div>
    <div class="p-8 max-w-lg mx-autorounded-xl shadow-lg space-y-6">
      <!-- Header -->
      <h1 class="text-2xl font-bold text-center">Story Details</h1>

      <!-- Title -->
      <div>
        <label for="title" class="block text-sm font-semibold mb-1"
          >Title</label
        >
        <input
          type="text"
          v-model="title"
          placeholder="Enter the title of your story"
          class="border block w-full p-3 rounded-lg"
        />
      </div>

      <!-- Genre -->
      <div>
        <label for="genre" class="block text-sm font-semibold mb-1"
          >Genre</label
        >
        <select
          v-model="selectedGenre"
          id="genre"
          class="border block w-full p-3 rounded-lg"
        >
          <option value="">Please choose</option>
          <option
            v-for="genre in genres"
            :key="genre.value"
            :value="genre.value"
          >
            {{ genre.text }}
          </option>
        </select>
      </div>

      <!-- Premise -->
      <div>
        <label for="Premise" class="block text-sm font-semibold mb-1"
          >Premise</label
        >
        <input
          type="text"
          v-model="Premise"
          placeholder="Enter the premise of your story"
          class="border block w-full p-3 rounded-lg"
        />
      </div>

      <!-- Theme -->
      <div>
        <label for="Theme" class="block text-sm font-semibold mb-1"
          >Theme</label
        >
        <input
          type="text"
          v-model="Theme"
          placeholder="Enter the theme of your story"
          class="border block w-full p-3 rounded-lg"
        />
      </div>

      <!-- Lock Story Line -->
      <div>
        <label for="lsl" class="block text-sm font-semibold mb-1"
          >Lock Story Line</label
        >
        <input
          type="text"
          v-model="lsl"
          placeholder="Enter the lock story line"
          class="border block w-full p-3 rounded-lg"
        />
      </div>

      <!-- Log Line / Synopsis -->
      <div>
        <label for="ll" class="block text-sm font-semibold mb-1"
          >Log Line</label
        >
        <input
          type="text"
          v-model="ll"
          placeholder="Enter the log line or synopsis"
          class="border block w-full p-3 rounded-lg"
        />
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

// State variables
const title = ref("");
const selectedGenre = ref("");
const genres = [
  { value: "comedy", text: "Comedy" },
  { value: "action", text: "Action" },
  { value: "romantic", text: "Romantic" },
  { value: "scifi", text: "Sci-Fi" },
  { value: "fantasy", text: "Fantasy" },
  { value: "thriller", text: "Thriller" },
  { value: "horror", text: "Horror" },
  { value: "suspense", text: "Suspense" },
  { value: "historical", text: "Historical" },
];
</script>

<style></style>

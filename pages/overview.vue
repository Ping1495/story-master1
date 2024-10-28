<template>
  <div>
    <!-- Title -->
    <div>
      <label for="title">Title</label>
      <input type="text" v-model="title" class="border border-black" />
    </div>

    <!-- Genre -->
    <div>
      <label for="genre">Genre</label>
      <select v-model="selectedGenre" id="genre" class="border border-black">
        <option value="">Please choose</option>
        <option v-for="genre in genres" :key="genre.value" :value="genre.value">
          {{ genre.text }}
        </option>
      </select>
    </div>

    <!-- Premise -->
    <div>
      <label for="Premise">Premise</label>
      <input type="text" v-model="Premise" class="border border-black" />
    </div>

    <!-- Theme -->
    <!-- LOCK STORY LINE -->
    <!-- LOG LINE / Synopsis -->
    <!-- Character Profiles -->
    <!-- Inspiration/Reference -->
  </div>
</template>

<script setup>
import { ref } from "vue";

// State variables
const title = ref("");
const selectedGenre = ref("");
const genres = [
  { value: "comedy", text: "comedy" },
  { value: "action", text: "action" },
  { value: "romentic", text: "romentic" },
  { value: "scifi", text: "sci-fi" },
  { value: "fantasy", text: "fantasy" },
  { value: "thriller", text: "thriller" },
  { value: "horror", text: "horror" },
  { value: "suspense", text: "suspense" },
  { value: "historical", text: "historical" },
];
</script>

<style></style>

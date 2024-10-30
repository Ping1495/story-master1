<template>
  <div
    class="bg-gradient-to-b from-blue-900 to-blue-800 min-h-screen p-8 flex justify-center"
  >
    <div class="w-11/12">
      <!-- Header -->
      <div
        class="text-center text-5xl mb-12 text-yellow-400 font-extrabold tracking-wide underline decoration-yellow-400 decoration-4 underline-offset-4"
      >
        Story Details
      </div>

      <div class="shadow-lg rounded-2xl p-6 background-image">
        <div class="grid sm:grid-cols-6 grid-cols-1 gap-6">
          <!-- Title and Author -->
          <div
            class="sm:col-span-2 col-span-1 border border-blue-900 p-6 rounded-xl bg-gradient-to-b from-blue-900 to-blue-800 shadow-md"
          >
            <div class="pb-4">
              <label
                for="title"
                class="block text-lg font-bold mb-1 text-yellow-400"
                >Title</label
              >
              <input
                type="text"
                v-model="title"
                placeholder="ชื่อเรื่อง"
                class="border border-blue-800 block w-full p-3 focus:outline-none focus:ring-2 focus:ring-blue-600 hover:border-blue-800 transition"
              />
            </div>
            <label
              for="author"
              class="block text-lg font-bold mb-1 text-yellow-400"
              >by</label
            >
            <input
              type="text"
              v-model="author"
              placeholder="ผู้แต่ง"
              class="border border-blue-800 block w-full p-3 focus:outline-none focus:ring-2 focus:ring-blue-600 hover:border-blue-800 transition"
            />
          </div>

          <!-- Premise -->
          <div
            class="sm:col-span-4 col-span-1 border border-blue-900 p-6 rounded-xl bg-gradient-to-b from-blue-900 to-blue-800 shadow-md"
          >
            <label
              for="premise"
              class="block text-lg font-bold mb-1 text-yellow-400"
              >Premise</label
            >
            <textarea
              v-model="premise"
              placeholder="Enter the premise of your story"
              class="border border-blue-800 block w-full p-3 min-h-[100px] focus:outline-none focus:ring-2 focus:ring-blue-600 hover:border-blue-800 transition"
            ></textarea>
          </div>

          <!-- Main Genre -->
          <div
            class="sm:col-span-2 col-span-1 grid grid-cols-1 border border-blue-900 p-6 rounded-xl bg-gradient-to-b from-blue-900 to-blue-800 shadow-md"
          >
            <div class="pb-4">
              <label
                for="genre"
                class="block text-lg font-bold mb-1 text-yellow-400"
                >Main Genre</label
              >
              <select
                v-model="selectedGenre"
                id="genre"
                class="border border-blue-800 block w-full p-3 focus:outline-none focus:ring-2 focus:ring-blue-600 hover:border-blue-800 transition"
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

            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
              <div>
                <label
                  for="sub-genre-1"
                  class="block text-lg font-bold mb-1 text-yellow-400"
                  >Sub Genre 1</label
                >
                <select
                  v-model="selectedGenre1"
                  id="sub-genre-1"
                  class="border border-blue-800 block w-full p-3 focus:outline-none focus:ring-2 focus:ring-blue-600 hover:border-blue-800 transition"
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

              <div>
                <label
                  for="sub-genre-2"
                  class="block text-lg font-bold mb-1 text-yellow-400"
                  >Sub Genre 2</label
                >
                <select
                  v-model="selectedGenre2"
                  id="sub-genre-2"
                  class="border border-blue-800 block w-full p-3 focus:outline-none focus:ring-2 focus:ring-blue-600 hover:border-blue-800 transition"
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
            </div>
          </div>

          <!-- Theme -->
          <div
            class="sm:col-span-4 border border-blue-900 p-6 rounded-xl bg-gradient-to-b from-blue-900 to-blue-800 shadow-md"
          >
            <label
              for="theme"
              class="block text-lg font-bold mb-1 text-yellow-400"
              >Theme</label
            >
            <textarea
              v-model="theme"
              placeholder="Enter the theme of your story"
              class="border border-blue-800 block w-full p-3 min-h-[100px] focus:outline-none focus:ring-2 focus:ring-blue-600 hover:border-blue-800 transition"
            ></textarea>
          </div>

          <!-- Lock Story Line -->
          <div
            class="sm:col-span-6 border border-blue-900 p-6 rounded-xl bg-gradient-to-b from-blue-900 to-blue-800 shadow-md"
          >
            <label
              for="lock-story-line"
              class="block text-lg font-bold mb-1 text-yellow-400"
              >Lock Story Line</label
            >
            <textarea
              v-model="lockStoryLine"
              placeholder="Enter the lock story line"
              class="border border-blue-800 block w-full p-3 min-h-[100px] focus:outline-none focus:ring-2 focus:ring-blue-600 hover:border-blue-800 transition"
            ></textarea>
          </div>

          <!-- Log Line / Synopsis -->
          <div
            class="sm:col-span-4 border border-blue-900 p-6 rounded-xl bg-gradient-to-b from-blue-900 to-blue-800 shadow-md"
          >
            <label
              for="log-line"
              class="block text-lg font-bold mb-1 text-yellow-400"
              >Synopsis</label
            >
            <textarea
              v-model="logLine"
              placeholder="Enter the synopsis"
              class="border border-blue-800 block w-full p-3 min-h-[100px] focus:outline-none focus:ring-2 focus:ring-blue-600 hover:border-blue-800 transition"
            ></textarea>
          </div>
        </div>

        <!-- Submit Buttons -->
        <div class="flex justify-end mt-8">
          <button
            class="text-white bg-gradient-to-r from-blue-500 to-blue-700 font-semibold py-3 px-6 rounded-full shadow-lg hover:shadow-xl hover:from-blue-600 hover:to-blue-800 transition duration-200 transform hover:scale-105 active:scale-95"
            @click="saveStory"
          >
            Save Story
          </button>
          <button
            class="text-white bg-gradient-to-r from-orange-500 to-orange-700 font-semibold py-3 px-6 rounded-full shadow-lg hover:shadow-xl hover:from-orange-600 hover:to-orange-800 transition duration-200 transform hover:scale-105 active:scale-95 ml-4"
            @click="nextStep"
          >
            Next Step
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

// State variables
const title = ref("");
const selectedGenre = ref("");
const selectedGenre1 = ref("");
const selectedGenre2 = ref("");
const premise = ref("");
const theme = ref("");
const lockStoryLine = ref("");
const logLine = ref("");

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

// Dummy methods for saving and moving to the next step
function saveStory() {
  alert("Story saved!");
}

function nextStep() {
  alert("Moving to the next step!");
}
</script>

<style scoped>
.background-image {
  background-image: url("/public/city.jpg"); /* ใส่ URL ของภาพที่ต้องการใช้ */
  background-size: cover; /* หรือใช้ contain ขึ้นอยู่กับผลลัพธ์ที่ต้องการ */
  background-position: center; /* จัดตำแหน่งภาพให้อยู่ตรงกลาง */
  background-repeat: no-repeat; /* ไม่ให้ภาพซ้ำ */
}
.background-image2 {
  background-image: url("/public/city.jpg"); /* ใส่ URL ของภาพที่ต้องการใช้ */
  background-size: cover; /* หรือใช้ contain ขึ้นอยู่กับผลลัพธ์ที่ต้องการ */
  background-position: center; /* จัดตำแหน่งภาพให้อยู่ตรงกลาง */
  background-repeat: no-repeat; /* ไม่ให้ภาพซ้ำ */
}
</style>

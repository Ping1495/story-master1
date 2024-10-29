<template>
  <div
    class="flex justify-center py-16 bg-gradient-to-b from-blue-900 to-blue-800 min-h-screen"
  >
    <div class="w-11/12 max-w-screen-xl">
      <div
        class="text-center text-5xl mb-12 text-yellow-300 font-extrabold tracking-wide underline decoration-yellow-400 decoration-4 underline-offset-4"
      >
        Your Story
      </div>
      <div
        class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-2 lg:grid-cols-4 xl:grid-cols-5 gap-6"
      >
        <!-- Add New Project Button -->
        <div
          class="relative border border-yellow-400 rounded-lg overflow-hidden shadow-lg transition-transform duration-300 transform hover:scale-105 hover:shadow-2xl bg-yellow-400 hover:bg-yellow-300"
        >
          <div
            class="h-48 flex flex-col justify-center items-center p-4 text-center text-blue-900 font-extrabold text-2xl leading-relaxed tracking-wide space-y-2"
          >
            <span class="text-5xl animate-bounce">＋</span>
            <span>Add New Project</span>
          </div>
          <!-- Decorative Shine Effect -->
          <div
            class="absolute top-0 left-0 w-full h-full bg-gradient-to-r from-transparent to-yellow-200 opacity-0 hover:opacity-30 transition-opacity duration-300"
          ></div>
        </div>

        <!-- Project Cards with Animated Gradient Border -->
        <div
          v-for="i in 12"
          :key="i"
          class="relative border border-yellow-400 rounded-lg overflow-hidden shadow-lg transition-transform duration-300 transform hover:scale-105 hover:shadow-2xl bg-gradient-to-t from-blue-900 to-blue-800 hover:from-blue-800 hover:to-blue-700"
        >
          <div
            class="h-48 flex justify-center items-center p-4 text-center text-yellow-400 font-semibold text-lg leading-relaxed tracking-wide"
          >
            Lorem ipsum dolor sit amet consectetur.
          </div>
          <!-- Animated Border -->
          <div
            class="absolute inset-0 rounded-lg border-2 border-yellow-400 animate-border-glow"
          ></div>
          <!-- Decorative Dots -->
          <div
            class="absolute top-2 left-2 w-4 h-4 bg-yellow-300 rounded-full opacity-40 animate-bounce-slow"
          ></div>
          <div
            class="absolute bottom-2 right-2 w-6 h-6 bg-yellow-300 rounded-full opacity-20 animate-bounce-slower"
          ></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
@keyframes bounce-slow {
  0%,
  100% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-8px);
  }
}

@keyframes bounce-slower {
  0%,
  100% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-4px);
  }
}

.animate-bounce-slow {
  animation: bounce-slow 3s infinite;
}

.animate-bounce-slower {
  animation: bounce-slower 4s infinite;
}
</style>

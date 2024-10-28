<template>
  <div class="min-h-screen bg-gray-100 flex flex-col">
    <!-- Main Content -->
    <main class="flex-grow p-6">
      <section class="text-center">
        <h2 class="text-2xl font-semibold mb-4">
          Welcome to Your Health Tracker
        </h2>
        <p class="mb-6">
          Track your health, diet, and fitness easily with our intuitive
          interface.
        </p>
        <a
          href="#"
          class="bg-blue-600 text-white py-2 px-4 rounded hover:bg-blue-500"
          >Get Started</a
        >
      </section>

      <!-- Features Section -->
      <section class="mt-10 grid grid-cols-1 md:grid-cols-3 gap-6">
        <div class="bg-white p-4 shadow rounded-lg">
          <h3 class="font-bold text-xl">Track Your Workouts</h3>
          <p>Log your exercises and monitor your progress over time.</p>
        </div>
        <div class="bg-white p-4 shadow rounded-lg">
          <h3 class="font-bold text-xl">Monitor Your Diet</h3>
          <p>Keep track of your meals and calorie intake easily.</p>
        </div>
        <div class="bg-white p-4 shadow rounded-lg">
          <h3 class="font-bold text-xl">Sleep Analysis</h3>
          <p>Analyze your sleep patterns to improve your rest quality.</p>
        </div>
      </section>
    </main>
  </div>
</template>

<script setup>
// Place any setup logic here if needed
</script>

<style>
/* You can add additional styles if needed */
</style>

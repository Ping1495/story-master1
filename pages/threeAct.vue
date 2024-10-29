<template>
  <div
    class="flex justify-center items-center min-h-screen bg-gradient-to-b from-blue-900 to-blue-800 p-6"
  >
    <div class="w-10/12 bg-white shadow-xl rounded-lg p-8 space-y-6">
      <!-- Title Section -->
      <div
        class="text-center text-4xl font-extrabold tracking-wide text-blue-900 underline decoration-blue-900 decoration-4 underline-offset-4"
      >
        3 Act Structure
      </div>

      <div class="flex flex-col gap-8">
        <!-- Act 1 Setup -->
        <div>
          <div class="text-xl font-semibold text-blue-900 mb-1">
            Act 1: Setup
          </div>
          <p class="text-blue-950 mb-2">
            เป็นการแนะนำตัวละครหลัก เรื่องราว และฉาก
            เพื่อให้ผู้ชมเข้าใจบริบทของเรื่อง
          </p>
          <textarea
            placeholder="Describe the setup of your story here..."
            class="border border-blue-400 rounded-lg w-full min-h-[150px] p-4 focus:outline-none focus:ring-2 focus:ring-blue-800"
          ></textarea>
        </div>

        <!-- Act 2 Conflict -->
        <div>
          <div class="text-xl font-semibold text-blue-900 mb-1">
            Act 2: Conflict
          </div>
          <p class="text-blue-950 mb-2">
            แสดงถึงความขัดแย้งและปัญหาที่ตัวละครต้องเผชิญ
            ซึ่งจะสร้างแรงดึงดูดให้ผู้ชมติดตามต่อไป
          </p>
          <textarea
            placeholder="Describe the conflict of your story here..."
            class="border border-blue-400 rounded-lg w-full min-h-[150px] p-4 focus:outline-none focus:ring-2 focus:ring-blue-800"
          ></textarea>
        </div>

        <!-- Act 3 Resolution -->
        <div>
          <div class="text-xl font-semibold text-blue-900 mb-1">
            Act 3: Resolution
          </div>
          <p class="text-blue-950 mb-2">
            สรุปเรื่องราวและแก้ไขปัญหาต่างๆ ที่เกิดขึ้นใน Act 2
            โดยนำเสนอบทสรุปที่น่าพอใจ
          </p>
          <textarea
            placeholder="Describe the resolution of your story here..."
            class="border border-blue-400 rounded-lg w-full min-h-[150px] p-4 focus:outline-none focus:ring-2 focus:ring-blue-800"
          ></textarea>
        </div>
      </div>

      <div class="text-end">
        <button
          class="text-xl font-semibold text-white mb-2 border-2 px-9 py-2 bg-blue-800 hover:bg-blue-700 hover:border-blue-700 transition-colors duration-300 rounded-xl"
        >
          save
        </button>
        <button
          class="text-xl font-semibold text-white mb-2 border-2 px-9 py-2 bg-blue-800 hover:bg-blue-700 hover:border-blue-700 transition-colors duration-300 rounded-xl"
        >
          next
        </button>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style></style>

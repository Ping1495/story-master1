<template>
  <div>
    <div class="flex flex-col justify-center items-center py-5 h-[821px]">
      <div
        class="w-[350px] border border-black rounded-md flex flex-col pt-8 pb-8 gap-3"
      >
        <div class="text-center font-medium text-xl mb-3">REGISTER</div>
        <!-- username -->
        <div class="px-6">
          <div class="font-medium">Username</div>
          <input
            type="text"
            class="border-black border w-full rounded-full h-[35px] mt-1 px-4"
            placeholder="Harley Quinn"
          />
        </div>
        <!-- password -->
        <div class="px-6">
          <div class="font-medium">Password</div>
          <input
            type="text"
            class="border-black border w-full rounded-full h-[35px] mt-1 px-4"
            placeholder="Password123456"
          />
        </div>

        <!-- confirm password -->
        <div class="px-6">
          <div class="font-medium">Confirm Password</div>
          <input
            type="text"
            class="border-black border w-full rounded-full h-[35px] mt-1 px-4"
            placeholder="Password123456"
          />
        </div>

        <div class="text-center">
          <div class="pb-2">
            <p class="text-center m-2 text-base text-gray-600">
              Don't have an account?
              <NuxtLink to="/login" class="text-blue-900 hover:underline"
                >Login</NuxtLink
              >
            </p>
          </div>
          <button class="bg-blue-900 w-fit text-white px-10 py-2 rounded-md">
            Register
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

const username = ref("");
const password = ref("");
const confirmPassword = ref("");

const handleLogin = () => {
  // ดำเนินการล็อกอินที่นี่ (เช่น เรียก API)
  console.log(`Username: ${username.value}, Password: ${password.value}`);
};
</script>

<style>
/* คุณสามารถเพิ่มสไตล์ที่ต้องการได้ที่นี่ */
</style>

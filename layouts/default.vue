<template>
  <div class="w-full">
    <NavBar />
    <NuxtPage />
    <!-- <Footer /> -->
  </div>
</template>

<script setup>
import NavBar from "@/components/navbar.vue"; // นำเข้า NavBar
import Footer from "@/components/footer.vue"; // นำเข้า Footer ให้ใช้ตัวอักษรใหญ่
</script>

<style>
/* คุณสามารถเพิ่มสไตล์ที่ต้องการได้ที่นี่ */
</style>

<template>
  <div class="flex justify-center py-10 background-image">
    <div class="w-11/12">
      <div class="text-center text-5xl mb-4 text-white font-bold tracking-wide">
        Character Profile
      </div>
      <div class="p-6 text-black">
        <div class="grid grid-cols-1 xl:grid-cols-2 gap-6">
          <!-- Birth Info Section -->
          <div :class="boxStyel">
            <h2 :class="topicStyel">ข้อมูลทั่วไป</h2>
            <div class="grid sm:grid-cols-2 grid-cols-1 gap-x-2">
              <label class="block">
                บทบาทตัวละคร:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                ชื่อเล่น/ตัวละครอื่นๆเรียกว่า:
                <input type="text" :class="inputStyle" />
              </label>

              <label class="block">
                ชื่อเต็ม:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                นามสกุล:
                <input type="text" :class="inputStyle" />
              </label>

              <label class="block sm:col-span-2">
                เหตุผล/ความหมายของชื่อ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                วันเกิด:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                ราศี:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                กรุ๊ปเลือด:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                Biological Sex เพศทางร่างกาย:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                Gender Identity เพศทางจิตใจ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                Sexual Orientation รสนิยมทางเพศ:
                <input type="text" :class="inputStyle" />
              </label>
            </div>
          </div>

          <!-- Physical Appearance Section -->
          <div :class="boxStyel">
            <h2 :class="topicStyel">ลักษณะทางกายภาพ</h2>
            <div class="grid sm:grid-cols-2 grid-cols-1 gap-x-2">
              <label class="block">
                อายุ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                เขา/เธอดูเหมือนคนอายุ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                ความสูง:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                น้ำหนัก:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                รูปร่าง:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                สุขภาพ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                เชื้อชาติ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                สัญชาติ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                ลักษณะที่โดดเด่น:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                ตำหนิ รอยแผลเป็น หรือปาน:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block sm:col-span-2">
                ลักษณะภายนอกโดยรวม:
                <input type="text" :class="inputStyle" />
              </label>
            </div>
          </div>

          <!-- Likes & Dislikes Section -->
          <div :class="boxStyel2">
            <h2 :class="topicStyel">สิ่งที่ชอบและไม่ชอบ</h2>
            <div class="grid sm:grid-cols-2 grid-cols-1 gap-x-2">
              <label class="block">
                สิ่งที่เขา/เธอชอบที่สุด:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                สิ่งที่เขา/เธอเกลียดที่สุด:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                สีที่ชอบ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                สีที่ไม่ชอบ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                อาหารที่ชอบ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                อาหารที่ไม่ชอบ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block col-sp">
                เพลงที่ชอบ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                หนังสือที่ชอบ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                ภาพยนตร์ที่ชอบ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                สถานที่ที่ชอบ:
                <input type="text" :class="inputStyle" />
              </label>

              <label class="block sm:col-span-2">
                กิจกรรม/งานอดิเรกที่ชอบ:
                <input type="text" :class="inputStyle" />
              </label>
            </div>
          </div>

          <!-- Family Section -->
          <div :class="boxStyel2">
            <h2 :class="topicStyel">ครอบครัว</h2>
            <div class="grid sm:grid-cols-2 grid-cols-1 gap-x-2">
              <label class="block">
                ชื่อแม่:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                ความสัมพันธ์กับแม่:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                ชื่อพ่อ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                ความสัมพันธ์กับพ่อ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                ญาติอื่นๆ/ผู้เลี้ยงดู:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                อาศัยอยู่กับ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                พี่น้อง:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                เป็นลูกคนที่:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                ความสัมพันธ์กับพี่น้อง:
                <input type="text" :class="inputStyle" />
              </label>

              <label class="block">
                ความสัมพันธ์ครอบครัวโดยรวม:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block sm:col-span-2">
                สิ่งที่ทำให้ความสัมพันธ์กับครอบครัวเป็นแบบนั้น:
                <input type="text" :class="inputStyle" />
              </label>
            </div>
          </div>

          <!-- Background Section -->
          <div :class="boxStyel3">
            <h2 :class="topicStyel">พื้นหลัง</h2>
            <div class="grid sm:grid-cols-2 grid-cols-1 gap-x-2">
              <label class="block sm:col-span-2">
                บ้านเกิด:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block sm:col-span-2">
                ความรู้สึกที่มีกับวัยเด็ก:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block sm:col-span-2">
                ความทรงจำที่มีค่า:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block sm:col-span-2">
                เหตุการณ์วัยเด็กที่ยังส่งผลต่อเขา/เธอ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block sm:col-span-2">
                การศึกษา:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                ศาสนาของครอบครัว:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                ศาสนาของตัวละคร:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block sm:col-span-2">
                ปรัชญา/ความเชื่อ:
                <input type="text" :class="inputStyle" />
              </label>
            </div>
          </div>

          <!-- Personality Section -->
          <div :class="boxStyel3">
            <h2 :class="topicStyel">ตัวตน</h2>
            <div class="grid sm:grid-cols-2 grid-cols-1 gap-x-2">
              <label class="block sm:col-span-2">
                นิสัย:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                MBTI:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block">
                Enneagram ลักษณ์:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block sm:col-span-2">
                จุดอ่อน:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block sm:col-span-2">
                จุดแข็ง:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block sm:col-span-2">
                ความใฝ่ฝัน/สิ่งที่เขา/เธอต้องการทำหรือเป็น:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block sm:col-span-2">
                ความต้องการภายใน(dramatic need):
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block sm:col-span-2">
                สรุปตัวละคร:
                <input type="text" :class="inputStyle" />
              </label>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const topicStyel =
  "text-2xl py-2 font-medium   text-center text-white bg-gradient-to-r from-blue-600 to-red-600 rounded-xl mb-4";
const inputStyle =
  "block w-full border border-gray-300 rounded p-2 mb-4 focus:outline-none focus:border-blue-500 mt-2";
const boxStyel = "bg-gradient-to-t from-violet-100 to-red-100 p-4 rounded-lg ";
const boxStyel2 = "bg-gradient-to-t from-violet-100 to-red-100 p-4 rounded-lg ";
const boxStyel3 = "bg-gradient-to-t from-violet-100 to-red-100 p-4 rounded-lg ";
</script>

<style scoped>
.background-image {
  background-image: url("/public/lighthouse.jpg"); /* ใส่ URL ของภาพที่ต้องการใช้ */
  background-size: cover; /* หรือใช้ contain ขึ้นอยู่กับผลลัพธ์ที่ต้องการ */
  background-position: center; /* จัดตำแหน่งภาพให้อยู่ตรงกลาง */
  background-repeat: no-repeat; /* ไม่ให้ภาพซ้ำ */
}
</style>

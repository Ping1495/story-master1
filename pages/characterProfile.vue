<template>
  <div class="flex justify-center py-10 bg-gray-100">
    <div class="w-10/12 bg-white rounded-lg shadow-lg">
      <div class="text-4xl text-center font-bold text-gray-800 p-4 border-b">
        Character Profile
      </div>
      <div class="p-6">
        <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
          <!-- Birth Info Section -->
          <div class="bg-gray-50 p-4 rounded-lg shadow">
            <h2 class="text-lg font-semibold text-gray-700 mb-2">
              ข้อมูลทั่วไป
            </h2>
            <div class="grid grid-cols-2 gap-x-2">
              <label class="block mb-2">
                บทบาทตัวละคร:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                ชื่อเล่น:
                <input type="text" :class="inputStyle" />
              </label>

              <label class="block mb-2">
                ชื่อเต็ม:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                นามสกุล:
                <input type="text" :class="inputStyle" />
              </label>

              <label class="block mb-2 col-span-2">
                เหตุผล/ความหมายของชื่อ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                วันเกิด:
                <input type="date" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                ราศี:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                MBTI:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                Enneagram ลักษณ์:
                <input type="text" :class="inputStyle" />
              </label>
            </div>
          </div>

          <!-- Physical Appearance Section -->
          <div class="bg-gray-50 p-4 rounded-lg shadow">
            <h2 class="text-lg font-semibold text-gray-700 mb-2">
              ลักษณะทางกายภาพ
            </h2>
            <div class="grid grid-cols-2 gap-x-2">
              <label class="block mb-2">
                อายุ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                เขา/เธอดูเหมือนคนอายุ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                เชื้อชาติ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                สัญชาติ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                ตำหนิ รอยแผลเป็น หรือปาน:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                ลักษณะที่โดดเด่น:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                ความสูง:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                น้ำหนัก:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                รูปร่าง:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                สุขภาพ:
                <input type="text" :class="inputStyle" />
              </label>
            </div>
          </div>

          <!-- Likes & Dislikes Section -->
          <div class="bg-gray-50 p-4 rounded-lg shadow">
            <h2 class="text-lg font-semibold text-gray-700 mb-2">
              สิ่งที่ชอบและไม่ชอบ
            </h2>
            <div class="grid grid-cols-2 gap-x-2">
              <label class="block mb-2">
                สิ่งที่เขา/เธอชอบที่สุด:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                สิ่งที่เขา/เธอเกลียดที่สุด:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                สีที่ชอบ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                สีที่ไม่ชอบ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                อาหารที่ชอบ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                อาหารที่ไม่ชอบ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2 col-sp">
                เพลงที่ชอบ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                หนังสือที่ชอบ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                ภาพยนตร์ที่ชอบ:
                <input type="text" :class="inputStyle" />
              </label>
              <label class="block mb-2">
                สถานที่ที่ชอบ:
                <input type="text" :class="inputStyle" />
              </label>

              <label class="block mb-2 col-span-2">
                กิจกรรมที่ชอบ:
                <input type="text" :class="inputStyle" />
              </label>
            </div>
          </div>

          <!-- Family Section -->
          <div class="bg-gray-50 p-4 rounded-lg shadow">
            <h2 class="text-lg font-semibold text-gray-700 mb-2">ครอบครัว</h2>
            <label class="block mb-2">
              ชื่อแม่:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              ความสัมพันธ์กับแม่:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              ชื่อพ่อ:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              ความสัมพันธ์กับพ่อ:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              พ่อแม่เลี้ยง:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              อาศัยอยู่กับ:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              พี่น้อง:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              เป็นลูกคนที่:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              ความสัมพันธ์กับพี่น้อง:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              ญาติอื่นๆ:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              ความใกล้ชิดกับครอบครัว:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              ด้วยเหตุผล:
              <input type="text" :class="inputStyle" />
            </label>
          </div>

          <!-- Background Section -->
          <div class="bg-gray-50 p-4 rounded-lg shadow">
            <h2 class="text-lg font-semibold text-gray-700 mb-2">พื้นหลัง</h2>
            <label class="block mb-2">
              บ้านเกิด:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              ความรู้สึกที่มีกับวัยเด็ก:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              ความทรงจำแรก:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              เหตุการณ์วัยเด็กที่ยังส่งผลต่อเขา/เธอ:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              การศึกษา:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              ศาสนาของครอบครัว:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              ศาสนาของตัวละคร:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              ปรัชญาชีวิต:
              <input type="text" :class="inputStyle" />
            </label>
          </div>

          <!-- Personality Section -->
          <div class="bg-gray-50 p-4 rounded-lg shadow">
            <h2 class="text-lg font-semibold text-gray-700 mb-2">บุคลิกภาพ</h2>
            <label class="block mb-2">
              ลักษณะเด่น:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              อารมณ์:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              ลักษณะอื่นๆ:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              จุดอ่อน:
              <input type="text" :class="inputStyle" />
            </label>
            <label class="block mb-2">
              จุดแข็ง:
              <input type="text" :class="inputStyle" />
            </label>
          </div>

          <!-- Other Details Section -->
          <div class="bg-gray-50 p-4 rounded-lg shadow">
            <h2 class="text-lg font-semibold text-gray-700 mb-2">
              รายละเอียดอื่นๆ
            </h2>

            <label class="block mb-2">
              ความฝัน:
              <input type="text" :class="inputStyle" />
            </label>

            <label class="block mb-2">
              สิ่งที่เขา/เธอต้องการเป็น:
              <input type="text" :class="inputStyle" />
            </label>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      inputStyle:
        "block w-full border border-gray-300 rounded p-2 mb-4 focus:outline-none focus:border-blue-500",
    };
  },
};
</script>

<style scoped>
/* Add any additional custom styles here */
</style>

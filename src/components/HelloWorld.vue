<template>
  <div class="hello">
    <header>
      <h1 v-motion-slide-bottom class="text-center pt-96 text-white text-6xl">
        مكتب عين
        <span v-motion-slide-bottom class="text-yellow-600 rounded-xl">.</span>
      </h1>
      <h2
        v-motion-slide-bottom
        class="text-center pt-7 tracking-wider text-white text-4xl"
      >
        لجميع أنواع التأشيرات
      </h2>
    </header>
    <section
      v-motion
      :initial="{
        opacity: 0,
        y: 200,
      }"
      :visible="{
        opacity: 1,
        y: 0,
        delay: 900,
      }"
      class="my-10 flex flex-col items-center"
    >
      <p class="text-3xl lg:text-7xl md:text-6xl text-yellow-700">
        وَأَتِمُّوا الْحَجَّ وَالْعُمْرَةَ لِلَّهِ
      </p>
      <div class="quran">
        <img class="" src="../assets/images/Quran.png" alt="" />
      </div>
    </section>
    <section
      v-motion
      :initial="{
        opacity: 0,
        y: 200,
      }"
      :visible="{
        opacity: 1,
        y: 0,
        delay: 900,
      }"
      class="my-10 sm:mx-0 md:mx-5 lg:mx-32 flex flex-col items-center lg:flex-row justify-evenly"
    >
      <div
        v-motion
        :initial="{
          opacity: 0,
          x: 200,
        }"
        :visible="{
          opacity: 1,
          x: 0,
          delay: 900,
        }"
        class="text p-1 lg:p-7 md:p-7 rounded-xl mx-20 mb-7"
      >
        <h2 class="text-3xl text-yellow-700">مكتب عين</h2>
        <p class="text-xl pt-5 list-disc">لخدمات الحج والعمرة</p>
        <li class="my-3 text-xl">برامج متنوعة.</li>
        <li class="my-3 text-xl">فنادق مميزة.</li>
        <li class="my-3 text-xl">طيران أسيوط و سوهاج.</li>
      </div>
      <div>
        <img
          class="rounded-3xl mr-auto"
          src="../assets/images/hujaaj.jpg"
          alt=""
        />
      </div>
    </section>
    <section
      v-motion
      :initial="{
        opacity: 0,
        y: 200,
      }"
      :visible="{
        opacity: 1,
        y: 0,
        delay: 900,
      }"
      class="hadith__section my-28 mx-5 py-20 flex flex-col items-center"
    >
      <h2 class="text-3xl lg:text-5xl md:text-6xl text-yellow-500">
        قَالَ رَسُولَ اللَّهِ ﷺ
      </h2>
      <p
        class="text-white text-center mt-6 text-3xl lg:text-3xl md:text-6xl leading-10"
      >
        الْعُمْرَةُ إِلَى الْعُمْرَةِ كَفَّارَةٌ لِمَا بَيْنَهُمَا، وَالْحَجُّ
        الْمَبْرُورُ لَيْسَ لَهُ جَزَاءٌ إِلَّا الْجَنَّةَ
      </p>
    </section>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
  background-image: url(../assets/images/header2.jpg);
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
  background-repeat: no-repeat;
  padding-bottom: 25em;
}
.text {
  box-shadow: 0 0 4px 3px #553c09;
}

.hadith__section {
  background-image: url(../assets/images/kaba-cover.png);
  background-position: center;
  background-size: cover;
  background-attachment: fixed;
  background-repeat: no-repeat;
}
</style>

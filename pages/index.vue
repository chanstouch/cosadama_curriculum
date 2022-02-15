<template>
<div class="w-full">

  <Warning />

  <HeaderAlt />

  <!-- <div class="w-full bg-gradient-to-r from-slate-300 via-blue-200 to-slate-50">
      <Header />
      <div class="max-w-6xl py-20 md:py-28 px-5 md:px-20 mx-auto">
        <div class="text-2xl text-center md:text-left text-slate-600 font-semibold mb-9 leading-9 drop-shadow-sm">중앙대 비전공자 코딩 커뮤니티, <br> 코사다마의 <span class="underline-offset-2">오픈소스 커리큘럼</span>이 <br> 업로드되는 공간입니다.</div>
        <div class="flex justify-center md:block md:justify-start">
          <a href="https://cosadama.com" target="blank" class="drop-shadow-sm py-2.5 px-3 bg-transparent text-slate-500 rounded-lg border border-slate-400 text-sm hover:bg-slate-100 transition duration-200">자세히 알아보기</a>
        </div>
      </div>
  </div> -->

  <div class="bg-img section w-full py-40 sm:py-48 md:py-60 2xl:py-72 recruit-img relative"  style="background-image: url(team3.jpeg)">
  <div class="z-10 w-full h-full bg-gradient-to-t from-zinc-800 absolute bottom-0">
  <div class="z-40 absolute bottom-0 w-full">
    <div class="max-w-6xl px-5 mx-auto text-white drop-shadow-lg pb-7 md:pb-16">
      <div class="text-2xl md:text-3xl font-medium pb-3">커리큘럼은 코사다마가, <br class="inline md:hidden"> 공부는 스스로!</div>
      <div class="text-slate-300 keep-all text-sm md:text-base">오롯이 본인이 배움의 속도를 조절하세요. <br class="hidden md:inline"> 힘이 넘칠 때는 빠르게, 지칠 때는 조금씩 쉬어가도 좋습니다.</div>
    </div>
  </div>
  </div>

  </div>


  <div class="max-w-6xl mx-auto pt-9 md:pt-16 pb-12 md:pb-24 px-5">
    <div class="text-2xl text-slate-600 font-semibold mb-6 md:mb-10">커리큘럼</div>
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-x-5 gap-y-8">
      <div v-for='course of courses' :key="course">
        <nuxt-link :to='`${course.slug}/1-1`'>
          <div class="group">
            <div class="lead-box rounded-lg h-content mb-5">
              <img :src="require(`~/assets/resources/thumbnails/${course.image}`)" class="profile group-hover:scale-105 transition duration-300" alt="course thumbnail">
            </div>
            <div>
              <div class="text-slate-600 text-xl font-medium mb-2 group-hover:text-blue-500 transition duration-200">{{course.name}}</div>
              <div class="keep-all text-slate-500 mb-1.5">{{course.description}}</div>
              <div class="text-sm text-slate-400">커리 개발: {{course.authors[0]}} {{course.authors[1]}} {{course.authors[2]}} {{course.authors[3]}}</div>
            </div>
          </div>
        </nuxt-link>
      </div>
    </div>

  </div>

  <FooterFull />
</div>

</template>

<script>
export default {
    async asyncData({ $content, params }) {
        const courses = await $content('courses', params.id)
        .sortBy('order', 'asc')
        .fetch();
        return { courses }
    },
}
</script>

<style scoped>
.keep-all{
    word-break: keep-all;
}
.bg-img {
        background-position: center;
        background-repeat:  no-repeat;
        /* background-attachment: fixed; */
        background-size:  cover;
        background-color: #000000;
 }
.section {
  position: relative;
}
.inner {
  box-sizing: border-box;
  position: relative;
}
.keep-all {
  word-break: keep-all;
}
.lead-box {
    overflow: hidden;
}
.square-box {
    overflow: hidden;
}
.profile {
    object-fit: cover;
    /* overflow: hidden; */
}
</style>

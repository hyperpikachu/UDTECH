<template>
  <div class="q-pa-md">
    <q-carousel
      animated
      v-model="slide"
      navigation
      infinite
      :autoplay="autoplay"
      arrows
      transition-prev="slide-right"
      transition-next="slide-left"
      @mouseenter="autoplay = false"
      @mouseleave="autoplay = true"
    >
      <q-carousel-slide :name="1" img-src="https://cdn.quasar.dev/img/mountains.jpg" />
      <q-carousel-slide :name="2" img-src="https://cdn.quasar.dev/img/parallax1.jpg" />
      <q-carousel-slide :name="3" img-src="https://cdn.quasar.dev/img/parallax2.jpg" />
      <q-carousel-slide :name="4" img-src="https://cdn.quasar.dev/img/quasar.jpg" />
    </q-carousel>
  </div>

<div class="row justify-around q-gutter-xl">

  <div class="q-mt-xs">
    <div><h6 class="q-mb-none">유디테크</h6></div>
    <div>회사소개</div>
    <div>사업소개</div>
    <div>상품권</div>
    <div>쇼핑</div>
  </div>

   <div class="q-mt-xs">
    <div><h6 class="q-mb-none">회사소개</h6></div>
    <div>인사말</div>
    <div>연혁</div>
    <div>오시는길</div>
  </div>

   <div class="q-mt-xs">
    <div><h6 class="q-mb-none">사업소개</h6></div>
    <div>고객관리</div>
    <div>전화관리</div>
    <div>사무환경 개선</div>
  </div>

   <div class="q-mt-xs">
    <div><h6 class="q-mb-none">상품권</h6></div>
    <div>상품권 조회</div>
    <div>상품권 구매</div>
    <div>상품권 설정</div>
  </div>

  <div class="q-mt-xs">
    <div><h6 class="q-mb-none">쇼핑</h6></div>
    <div>오토큐 상품</div>
    <div>자동차 관리용품</div>
    <div>자동차 소모품</div>
    <div>상품권 구매</div>
  </div>
</div>

</template>

<style lang="scss">


</style>


<script>
import { ref } from 'vue'

export default {
  setup () {
    return {
      slide: ref(1),
      autoplay: ref(true)
    }
  }
}
</script>


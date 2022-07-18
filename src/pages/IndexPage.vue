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

  <div class="q-pa-md coldiv">

    <div class="column">
      <div class="col">유디테크</div>
      <div class="col">회사소개</div>
      <div class="col">사업소개</div>
      <div class="col">상품권</div>
      <div class="col">쇼핑</div>
    </div>

       <div class="column">
      <div class="col">회사소개</div>
      <div class="col">인사말</div>
      <div class="col">연혁</div>
      <div class="col">오시는길</div>
    </div>

    <div class="column">
      <div class="col">사업소개</div>
      <div class="col">고객관리</div>
      <div class="col">전화관리</div>
      <div class="col">사무환경 개선</div>
    </div>

     <div class="column">
      <div class="col">상품권</div>
      <div class="col">상품권조회</div>
      <div class="col">상품권구매</div>
      <div class="col">상품권설정</div>
    </div>

     <div class="column">
      <div class="col">쇼핑</div>
      <div class="col">오토큐상품</div>
      <div class="col">자동차 관리용품</div>
      <div class="col">자동차 소모품</div>
      <div class="col">상품권구매</div>
    </div>

  version1 css로 작업해봄


  </div>

</template>

<style scoped lang="scss">

.coldiv {
  display: flex;
  background-color:none;
  justify-content: center;
  align-items: flex-start;

}

.column {
  background-color: none;
  margin: 0px 45px;
  justify-content: flex-start;
  align-items: flex-start;
}

.col {
  width: 100px;
  height: 30px;
  margin: 0;
  box-sizing:border-box;
  margin-bottom: 10px;
}


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


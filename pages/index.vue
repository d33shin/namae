<template lang="pug">
  v-container
    div(class='mb-12')

      p {{ description }}
      p 영업시간은 오전 9시 부터 오후 10까지입니다.
      p(class='text-h5 font-weight-') 문의 🤙 010 4490 5566

    v-divider(class='my-12')

    div(class='mb-12')
      h1(class='text-h3 mb-6 text-center') 메뉴
      h2(class='mb-3 text-h4')  🍖 고기류
      p 정육점을 운영하고있어 매일매일 신선한 강원도 청정 고기를 제공합니다.

    v-row(class='mb-12')
      v-col(cols=12 sm=6)
        h3(class='text-h5 font-weight-bold') 삼겹살
        v-img(class='image' :src='require("@/assets/images/menu/삼겹살.jpg?resize&size=700&format=webp")' alt='삼겹살')
        p(class='mt-1') 1인분(200g) 13,000원
      v-col(cols=12 sm=6)
        h3(class='text-h5 font-weight-bold') 목살
        v-img(class='image' :src='require("@/assets/images/menu/목살.jpg?resize&size=700&format=webp")' alt='목살')
        p(class='mt-1') 1인분(200g) 13,000원   
      v-col(cols=12 sm=6)
        h3(class='text-h5 font-weight-bold') 오겹살
        v-img(class='image' :src='require("@/assets/images/menu/오겹살.jpg?resize&size=700&format=webp")' alt='오겹살')
        p(class='mt-1') 1인분(200g) 13,000원   
      v-col(cols=12 sm=6)
        h3(class='text-h5 font-weight-bold') 대패삼겹살
        v-img(class='image' :src='require("@/assets/images/menu/대패삼겹살.jpg?resize&size=700&format=webp")' alt='대패삼겹살')
        p(class='mt-1') 1인분(250g) 10,000원   

    v-divider(class='my-12') 

    h2(class='mb-3 text-h4') 🍗 치킨
    p 치킨은 포장메뉴입니다 미리전화주시면 기다리실 필요없이 바로 오셔서 픽업하세요 ⚡  
    v-row(class='mb-12')
      v-col(cols=12 sm=6)
        h3(class='text-h5 font-weight-bold') 옛날통닭
        v-img(class='image' :src='require("@/assets/images/menu/옛날통닭.jpg?resize&size=700&format=webp")' alt='옛날통닭')
        p(class='mt-1') 한마리 10,000원 / 두마리 18,000원
      v-col(cols=12 sm=6)
        h3(class='text-h5 font-weight-bold') 양념통닭
        v-img(class='image' :src='require("@/assets/images/menu/양념통닭.jpg?resize&size=700&format=webp")' alt='양념통닭')
        p(class='mt-1') 한마리 10,000원 / 두마리 18,000원
      v-col(cols=12 sm=6)
        h3(class='text-h5 font-weight-bold') 소스
        v-img(class='image' :src='require("@/assets/images/menu/소스.jpg?resize&size=700&format=webp")' alt='소스')
        p(class='mt-1') 머스타드, 매운소스 *각각 500원*
      v-col(cols=12 sm=6)
        h3(class='text-h5 font-weight-bold') 생맥주
        v-img(class='image' :src='require("@/assets/images/menu/맥주.jpg?resize&size=700&format=webp")' alt='맥주')
        p(class='mt-1') 1리터 8,000원
      v-col(cols=12 sm=6)
        h3(class='text-h5 font-weight-bold') 콜라
        v-img(class='image' :src='require("@/assets/images/menu/콜라.jpg?resize&size=700&format=webp")' alt='콜라')
        p(class='mt-1') 2,000원
    
    v-divider(class='my-12')

    h2(class='mb-3 text-h4') 🍲 식사류
    v-row
      v-col(cols=12 sm=6)
        h3(class='text-h5 font-weight-bold') 육개장
        v-img(class='image' :src='require("@/assets/images/menu/육개장.jpg?resize&size=700&format=webp")' alt='육개장')
        p(class='mt-1') 8,000원
      v-col(cols=12 sm=6)
        h3(class='text-h5 font-weight-bold') 설렁탕
        v-img(class='image' :src='require("@/assets/images/menu/설렁탕.jpg?resize&size=700&format=webp")' alt='설렁탕')
        p(class='mt-1') 8,000원
      v-col(cols=12 sm=6)
        h3(class='text-h5 font-weight-bold') 된장찌게
        v-img(class='image' :src='require("@/assets/images/menu/된장찌게.jpg?resize&size=700&format=webp")' alt='된장찌게')
        p(class='mt-1') 8,000원
      v-col(cols=12 sm=6)
        h3(class='text-h5 font-weight-bold') 제육덮밥
        v-img(class='image' :src='require("@/assets/images/menu/제육덮밥.jpg?resize&size=700&format=webp")' alt='제육덮밥')
        p(class='mt-1') 8,000원
      v-col(cols=12 sm=6)
        h3(class='text-h5 font-weight-bold') 해물덮밥
        v-img(class='image' :src='require("@/assets/images/menu/해물덮밥.jpg?resize&size=700&format=webp")' alt='해물덮밥')
        p(class='mt-1') 9,000원
    
    v-divider(class='my-12')

    div
      h2 🤙예약 문의
      p(class='font-weight-black text-h1') 010 4490 5566

</template>

<style lang="sass" scoped>
.image
  height: 380px
</style>

<script>
module.exports = {
  head() {
    return {
      title: this.title,
    };
  },
  data() {
    return {
      title: "남애항 정육식당 & 치킨",
      description: "남애항 정육식당 & 치킨의 메뉴입니다.",
    };
  },
};
</script>

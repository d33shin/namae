<template lang="pug">
  v-container
    div(class='mb-6')
      h1 메뉴
      p {{ description }}

    h2(class='mb-3')  🍖 고기류
    p 정육점을 운영하고있어 매일매일 신선한 강원도 청정 고기를 제공합니다.

    v-row(class='mb-6')
      v-col(cols=12 sm=6)
        h3 목살
        v-img(class='image' :src='require("@/assets/images/menu/목살.jpg?resize&size=700&format=webp")' alt='목살')
        p(class='mt-1') 1인분(200g) 13,000원   
      v-col(cols=12 sm=6)
        h3 삼겹살
        v-img(class='image' :src='require("@/assets/images/menu/삼겹살.jpg?resize&size=700&format=webp")' alt='삼겹살')
        p(class='mt-1') 1인분(200g) 13,000원

    h2(class='mb-3') 🍗 치킨
    p 치킨은 포장메뉴입니다 미리전화주시면 기다리실 필요없이 바로 오셔서 픽업하세요 ⚡  
    v-row(class='mb-6')
      v-col(cols=12 sm=6)
        h3 옛날통닭
        v-img(class='image' :src='require("@/assets/images/menu/옛날통닭.jpg?resize&size=700&format=webp")' alt='옛날통닭')
        p(class='mt-1') 한마리 10,000원 / 두마리 18,000원
      v-col(cols=12 sm=6)
        h3 양념통닭
        v-img(class='image' :src='require("@/assets/images/menu/옛날통닭.jpg?resize&size=700&format=webp")' alt='옛날통닭')
        p(class='mt-1') 한마리 10,000원 / 두마리 18,000원
      v-col(cols=12 sm=6)
        h3 소스
        v-img(class='image' :src='require("@/assets/images/menu/옛날통닭.jpg?resize&size=700&format=webp")' alt='옛날통닭')
        p(class='mt-1') 머스타드, 매운소스 *각각 500원*
      v-col(cols=12 sm=6)
        h3 생맥주
        v-img(class='image' :src='require("@/assets/images/menu/옛날통닭.jpg?resize&size=700&format=webp")' alt='옛날통닭')
        p(class='mt-1') 한마리 10,000원 / 두마리 18,000원
      v-col(cols=12 sm=6)
        h3 콜라
        v-img(class='image' :src='require("@/assets/images/menu/옛날통닭.jpg?resize&size=700&format=webp")' alt='옛날통닭')
        p(class='mt-1') 2,000원
    
    h2(class='mb-3') 🍲 식사류
    v-row
      v-col(cols=12 sm=6)
        h3 육개장
        v-img(class='image' :src='require("@/assets/images/menu/육개장.jpg?resize&size=700&format=webp")' alt='육개장')
        p(class='mt-1') 8,000원
      v-col(cols=12 sm=6)
        h3 설렁탕
        v-img(class='image' :src='require("@/assets/images/menu/설렁탕.jpg?resize&size=700&format=webp")' alt='설렁탕')
        p(class='mt-1') 8,000원
      v-col(cols=12 sm=6)
        h3 제육덮밥
        v-img(class='image' :src='require("@/assets/images/menu/제육덮밥.jpg?resize&size=700&format=webp")' alt='제육덮밥')
        p(class='mt-1') 8,000원
      v-col(cols=12 sm=6)
        h3 해물덮밥
        v-img(class='image' :src='require("@/assets/images/menu/해물덮밥.jpg?resize&size=700&format=webp")' alt='해물덮밥')
        p(class='mt-1') 9,000원
</template>

<style lang="sass" scoped>
.image
  height: 380px
</style>

<script>
module.exports = {
  head() {
    return {
      title: this.title
    };
  },
  data() {
    return {
      title: "메뉴",
      description: "남애항 정육식당 & 치킨의 메뉴입니다."
    };
  }
};
</script>

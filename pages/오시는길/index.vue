<template lang="pug">
  v-container
    div(class='my-12')
      h1(class='title text-h3 mb-4') 🚗 오시는길 📍
      p(class='text-h4') 강원도 양양군 현남면 매바위길 131
    h2(class='text-h4') 🤙 문의전화
    p(class='text-h4') 010 4490 5566
</template>

<script>
module.exports = {
  head() {
    return {
      title: this.title
    };
  },

  data() {
    return {
      title: "오시는길"
    };
  }
};
</script>

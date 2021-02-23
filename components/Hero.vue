<template lang="pug">
  v-row
    v-col(cols=6)
      v-img(:src="myImg(img, size)")
    v-col(cols=6)
      h1 {{ msg }}
</template>

<script>
export default {
  methods: {
    myImg(file, size) {
      const data = `@/assets/images/${file}?resize&size=${size}&format=webp`;
      return require(data);
    }
  },
  props: ["msg", "img", "size"]
};
</script>

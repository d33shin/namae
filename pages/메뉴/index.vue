<template lang="pug">
  v-container
    h1 메뉴
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
      title: "메뉴"
    };
  }
};
</script>

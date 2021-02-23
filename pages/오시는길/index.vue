<template lang="pug">
  v-container
    h1 오시는길
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

<template lang="pug">
  div
    ul
      li(
        v-for='vid in vids'
        :key='vid.title'
      ) {{ vid.snippet }}
        v-img(:src='require(`@/assets/images/${vid.cards[1].image}?resize&size=1000&format=webp`)')
</template>

<script>
var { mapState } = require("vuex");

module.exports = {
  head() {
    return {
      title: this.title
    };
  },
  data() {
    return {
      title: "Proposal for surfing and leisure business",
      msg: "This is the message from data..."
    };
  },
  computed: {
    ...mapState(["vids"])
  }
};
</script>

<template lang="pug">
  article
    nuxt-content(:document='post')
</template>

<script>
export default {
  async asyncData({ $content, params }) {
    const post = await $content("blog", params.slug).fetch();

    return { post };
  }
};
</script>

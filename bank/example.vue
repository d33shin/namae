<template>
  <div>
    <!-- single WebP image -->
    <img :src="oneSizeWebP.src" />

    <!-- single AVIF image -->
    <img :src="oneSizeAvif.src" />

    <!-- source set with multiple sizes -->
    <img :srcSet="multipleSizes.srcSet" :src="multipleSizes.src" />
  </div>
</template>

<script>
const oneSizeWebP = require('~/assets/my-image.jpg?resize&size=300&format=webp');
const oneSizeAvif = require('~/assets/my-image.jpg?resize&size=300&format=avif');
const multipleSizes = require('~/assets/my-image.jpg?resize&sizes[]=300&sizes[]=600&sizes[]=1000&format=webp');

export default {
  data() {
    return { oneSizeWebP, , oneSizeAvif, multipleSizes }
  }
}
</script>

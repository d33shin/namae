<template lang="pug">
  nav(class='scroll-y')

    v-navigation-drawer(v-model="drawer" app)
      v-list-item
        v-list-item-content
          v-list-item-title(class="title") 남애항 정육식당 &amp; 치킨
          v-list-item-subtitle 신선한 🍖, 바삭한 🍗

      v-divider

      v-list(dense nav)
        v-list-item(v-for="item in items" :key="item.title" :to="item.to" link)
          v-list-item-icon
            v-icon(color="pink") {{ item.icon }}
          v-list-item-content
            v-list-item-title {{ item.title }}


    v-app-bar(app color='blue-grey darken-4' flat)
     
        
      v-app-bar-nav-icon(
        color="pink"
        @click="drawer = !drawer"
      )
      
      v-toolbar-title
        v-img(:src='require("~/assets/images/logo-namae.svg")')

</template>

<script>
export default {
  data: () => ({
    drawer: false,
    items: [
      { title: "홈", icon: "mdi-star-face", to: "/" },
      { title: "오시는길", icon: "mdi-map-marker-radius", to: "/오시는길" }
    ],
    right: null
  }),
  methods: {
    onScroll(e) {
      if (typeof window === "undefined") return;
      const top = window.pageYOffset || e.target.scrollTop || 0;
      this.fab = top > 20;
    },
    toTop() {
      this.$vuetify.goTo(0);
    }
  }
};
</script>

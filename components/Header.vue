<template lang="pug">
  nav

    v-navigation-drawer(v-model="drawer" app)
      v-list-item
        v-list-item-content
          v-list-item-title(class="title") ABSYNTH
          v-list-item-subtitle Synthsise universe

      v-divider

      v-list(dense nav)
        v-list-item(v-for="item in items" :key="item.title" :to="item.to" link)
          v-list-item-icon
            v-icon(color="pink") {{ item.icon }}
          v-list-item-content
            v-list-item-title {{ item.title }}


    v-app-bar(app)
      v-app-bar-nav-icon(
        color="pink"
        @click="drawer = !drawer"
      )
      
      v-toolbar-title ABSYNTH

      v-spacer

      div(v-if="$auth.loggedIn")
        p {{ $auth.user.email }}
        v-btn(text to="/") Logout
        
      div(v-else)
        v-btn(text to="/login") Login
        v-btn(text to="/register") Register
</template>

<script>
export default {
  data: () => ({
    drawer: false,
    items: [
      { title: "Todo", icon: "mdi-star-face", to: "/" },
      { title: "About", icon: "mdi-waves", to: "/about" },
      { title: "Location", icon: "mdi-map-marker", to: "/location" },
      { title: "Contacts", icon: "mdi-at", to: "/contacts" }
    ],
    right: null
  })
};
</script>

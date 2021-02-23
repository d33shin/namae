<template lang="pug">
  v-container
    h1 Login

    UserAuthForm(buttonText='Login' :submitForm='loginUser')
</template>

<script>
export default {
  methods: {
    loginUser() {
      alert("You pressed the button");
    }
  }
};
</script>

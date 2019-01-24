<template>
  <div class="login">
    <h1>This is a login page</h1>
    <form @submit.prevent="login">
      Username: <input type ="text" v-model="username"><br>
      Password: <input type ="password" v-model="password"><br>
      <input type ="submit" value="Login">
    </form>
  </div>
</template>

<script>
export default {
  name: 'login',
  data: () => {
    return {
      username: "",
      password: ""
    }
  },
  methods: {
    login() {
      window.user = {
        username: this.username,
        password: this.password
      }
      this.$router.push('home')
    }
  }
}
</script>
<template>
  <div class="login-container">
    <h1>Login</h1>
    <input type="text" v-model="username" placeholder="Username" />
    <input type="password" v-model="password" placeholder="Password" />
    <button @click="login">Login</button>
  </div>
</template>

<script>
export default {
  name: 'LoginPage',
  data() {
    return { username: '', password: '' }
  },
  methods: {
    login() {
      // TODO: implement login
    }
  }
}
</script>

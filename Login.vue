<template>
  <div class="login-wrapper">
    <div class="login-card">
      <h2>Sign In</h2>
      <el-form :model="form" @submit.native.prevent="handleLogin">
        <el-form-item label="Username">
          <el-input v-model="form.username" />
        </el-form-item>
        <el-form-item label="Password">
          <el-input v-model="form.password" type="password" />
        </el-form-item>
        <el-button type="primary" native-type="submit">Sign In</el-button>
      </el-form>
    </div>
  </div>
</template>

<script>
export default {
  name: 'LoginPage',
  data() {
    return {
      form: { username: '', password: '' }
    }
  },
  methods: {
    handleLogin() {
      this.$router.push('/dashboard')
    }
  }
}
</script>

<script>
import LoginForm from '../components/LoginForm.vue';
export default { components: { LoginForm }, data() { return {} } };
</script>

<template>
  <div class="login-page">

    <LoginForm />
  </div>
</template>
<style>
.login-page {
  height: 95vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>

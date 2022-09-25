<script>
import InputField from './InputField.vue';

export default {
  components: {
    InputField
  },
  methods: {
    say(message) { alert(message) }
  }
}
</script>
<template>
  <div class="login-form">
    <h2>Welcome to the stealing party.. Let's get you logged in!</h2>
    <InputField label="E-mail" id="email" placeholder="E-mail" type="email" />
    <InputField label="Password" id="password" placeholder="Password" type="password" />
    <button class="login-btn" @click="say('hello')">Log in</button>
  </div>
</template>
<style>
.login-btn {
  width: 50%;
  margin-top: 20px;
  border: none;
  padding: 10px;
  border-radius: 4px;
  background-color: #05442f;
  color: #bdf2e2;
  box-shadow: rgba(0, 0, 0, 0.15) 1.95px 1.95px 2.6px;
}

.login-form {
  display: inline-block;
  width: 25%;
  padding: 100px;
  border: 2px solid #bdf2e2;
  border-radius: 4px;
  box-shadow: rgba(0, 0, 0, 0.15) 1.95px 1.95px 2.6px;
  background-color: white;
}
</style>

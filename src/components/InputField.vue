<script>
export default {
  props: {
    label: String,
    id: String,
    placeholder: String,
    type: String,
  }
}
</script>
<template>
  <div class="input">
    <input class="field" :id="id" :placeholder="placeholder" :type="type">
  </div>
</template>
<style>
.input {
  margin-top: 20px;
  margin-right: 20px;

}

.field {
  padding: 10px;
  min-width: 100%;
  border: none;
  background-color: #bdf2e2;
  border-radius: 4px;
  box-shadow: rgba(0, 0, 0, 0.15) 1.95px 1.95px 2.6px;
}
</style>

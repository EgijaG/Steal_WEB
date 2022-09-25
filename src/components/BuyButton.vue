<script>
export default {
  props: {
    displayPrice: Number,
  },
  data() {
    return {
      count: 0
    }
  }
}
</script>

<template>
  <button @click="count++">
    {{ displayPrice }} $
  </button>
</template>

<style>
button {
  background-color: #0C888E;
  color: #000;
  padding: 10px;
  border-radius: 4px;
  border: 0.5px solid #2D5354;
  font-family: 'Allerta', sans-serif;
  font-size: 15px;
}
</style>

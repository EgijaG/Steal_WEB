<script>
import BuyButton from './BuyButton.vue';
export default {
  components: { BuyButton },
  data() {
    return {
      title: 'Nudes',
      description: 'Loti good kvaliti'
    }
  }
}
</script>

<template>
  <div id="card">
    <img src="../assets/img/first.jpg" alt="">
    <h2>{{title}}</h2>
    <p>{{description}}</p>
    <BuyButton />
  </div>
</template>

<style>
#card {
  display: inline-block;
  padding: 10px;
  background-color: #ABCED2;
  border-radius: 4px;
  border: 0.5px solid #000;
  max-width: 25%;
  margin: 20px 10px;
}

img {
  max-width: 80%;
}
</style>

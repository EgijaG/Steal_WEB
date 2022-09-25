<script>
import BuyButton from './BuyButton.vue';

export default {
  components: { BuyButton },
  props: {
    title: String,
    description: String,
    price: Number,
    category: String
  },
  data() {
    return {

    }
  }
}
</script>

<template >
  <div id="card">
    <img src="../assets/img/first.jpg" alt="">
    <h3>{{title}}</h3>
    <p>{{description}}</p>
    <BuyButton :displayPrice="price" />
  </div>
</template>

<style>
#card {
  display: inline-block;
  padding: 20px 5px;
  background-color: #ABCED2;
  border-radius: 4px;
  max-width: 25%;
  margin: 20px 10px;
  /* filter: drop-shadow(10px 5px 10px grey); */
  box-shadow: rgba(46, 240, 195, 0.4) -5px 5px, rgba(46, 240, 195, 0.3) -10px 10px, rgba(46, 240, 204, 0.2) -15px 15px, rgba(46, 211, 240, 0.1) -20px 20px, rgba(46, 240, 230, 0.05) -25px 25px;
}

img {
  max-width: 80%;
  border-radius: 4px;
  margin-top: 5%;
}

p {
  font-family: 'Courier Prime', monospace;
  font-size: 20px;
}
</style>

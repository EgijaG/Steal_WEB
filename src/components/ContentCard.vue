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
  filter: drop-shadow(10px 5px 10px grey);
}

img {
  max-width: 80%;
  border-radius: 4px;
  margin-top: 5%;
}

p {
  font-family: 'Courier Prime', monospace;
  font-size: 24px;
}
</style>

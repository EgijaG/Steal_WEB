

<script>
import BuyButton from './components/BuyButton.vue';
import ContentCard from './components/ContentCard.vue';
import PageHeader from './components/PageHeader.vue';
import PageFooter from './components/PageFooter.vue';
import prodData from './data/products.json';
export default {
  name: 'app',
  components: {
    ContentCard,
    PageHeader,
    PageFooter
},

  data() {
    return {
      products: prodData,

    }

  }

}
</script>
<template>
  <div id="app">
    <PageHeader />
    <div v-for="p in products" class="cards">
      <ContentCard :title="p.name" :description="p.description" :price="p.price" />
    </div>
    <PageFooter />
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Merriweather+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700;1,800&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Great+Vibes&family=Merriweather+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700;1,800&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Allerta&display=swap%27);
@import url('https://fonts.googleapis.com/css2?family=Courier+Prime&display=swap%27);


#app {
  font-family: 'Allerta', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  flex: 1;
  padding-bottom: 40px;
  position: relative;
}

body {
  margin:0;
}

.cards {
  display: inline;
  max-width: 25%;

}

h1,
h2 {
  font-family: 'Courier Prime', monospace;
  font-weight: normal;
  font-size: 64px;
}

h3 {
  font-family: 'Allerta', sans-serif;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>

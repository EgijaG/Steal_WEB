

<script>
import BuyButton from './components/BuyButton.vue';
import ContentCard from './components/ContentCard.vue';
export default {
  name: 'app',
  components: {
    ContentCard
  },
  data() {
    return {
      msg: 'Hello world! This is a fantastic day!',
      script: 'This is lorem ipsum'
    }

  }

}
</script>
<template>
  <div id="app">
    <header></header>
    <h1>{{ msg }}</h1>
    <h3>{{script}}</h3>
    <ContentCard />
    <ContentCard />
    <ContentCard />
    <ContentCard />
    <ContentCard />
    <ContentCard />
    <footer></footer>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Merriweather+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700;1,800&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Great+Vibes&family=Merriweather+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700;1,800&display=swap');

#app {
  font-family: 'Merriweather Sans', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  flex: 1;
}

h1,
h2 {
  font-family: 'Great Vibes', cursive;
  font-weight: normal;
  font-size: 64px;
}

h3 {
  font-family: 'Merriweather Sans', sans-serif;
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

<template>
  <div id="app">
    <h1>Group Members and there Contribution</h1>
    <ItemDispay v-for="(item, index) in items" :key="index" :item="item" />
  </div>
</template>

<script>
import ItemDispay from './components/ItemDispay.vue';

export default {
  name: 'App',
  components: {
    ItemDispay
  },
  data() {
    return {
      items: [
        { name: 'Gavin Boris', price: '$1000' },
        { name: 'Uwizera Gael', price: '$150' },
        { name: 'Jules Kennedy', price: '$100' },
        { name: 'Joanna Micarla', price: '$250' }
      ]
    };
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

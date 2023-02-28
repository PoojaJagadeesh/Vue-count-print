<template>
  <div id="app">
  <div>
    <p v-for="i in count">{{ i }}</p>
    <button @click="add">Click</button>
    <div>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
  },
  data() {
    return {
      i: 0,
      count:0,
    };
  },
  methods:{
    add(){
     this.count++;
    }
  }
};
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

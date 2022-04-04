<template>
  <hello-world v-for="product in products" :key="product.id" :product="product"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
 
  name: 'App',
  components: {
    HelloWorld
  },
  data : () =>{
     return {
       products: [
      {
        id:"1",
        name:"Palmerita",
        url:"url",
      },
        {
        id:"2",
        name:"Palmerita2",
        url:"url",
      },
        {
        id:"3",
        name:"Palmerita3",
        url:"url",
      }

    ]
     }
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

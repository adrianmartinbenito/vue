<template>
<div class="card">
  <span>{{product.name}}</span>
  <span>{{product.url}}</span>
</div>
    
</template>

<script>

export default {
  
  name: 'HelloWorld',
  props: {
    product:{
      type:Object,
      default:null
    },
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
.card{
  display:flex;
  flex-direction:column;
}
</style>

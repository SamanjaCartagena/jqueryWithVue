<template>
<div>
<ul class="nav">
  <li class="active">
    <a href="#">Home</a>
  </li>
  <li><a href="#">Link</a></li>
  <li><a href="#">Link</a></li>
</ul>
</div>
  
</template>

<script>
import jquery from 'jquery'

export default {
  name: 'App',
  components: {
  },
  data(){
    return {

    }
  },
  mounted(){
    this.$nextTick(()=>{
      jquery('.nav').hide();
      jquery('.nav').fadeIn('slow');
    })
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
li{
  padding:20px;
}
</style>

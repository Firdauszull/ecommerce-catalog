<template>
  <ProductDisplay/>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </nav>
  <router-view/>

</template>



<style>
body{
    background-image: url("./assets/bg.png");
    background: cover;
    background-size: cover ;

 
 
}
*{box-shadow: border-box;}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>

<script>
import ProductDisplay from './components/ProductDisplay.vue'

export default{
  name :'App',
  components:{
    ProductDisplay
  }
}
  
</script>


<template>
  <div id="app">
    <Navbar_component/>
    <Carusel_wine/>
    <Product_component/>
    <wine_futer/>
  </div>
</template>

<script>

import Navbar_component from "@/components/navbar_component";
import Product_component from "@/components/product_component";
// import Carusel_wine from "@/components/carusel-wine"
import wine_futer from "@/components/wine_futer";

export default {
  name: 'App',
  components: {
    Product_component,
    Navbar_component,
    // Carusel_wine,
    wine_futer
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

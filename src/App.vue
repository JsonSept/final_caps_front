<template>
  <navbar-comp/>
  <spinner-comp/>
  <router-view/>
  <footer-comp/>
  <product-admin/>
</template>

<script>

import NavbarComp from './components/NavbarComp.vue'
import SpinnerComp from './components/SpinnerComp.vue'
import FooterComp from './components/FooterComp.vue'

 export default {
  components : {
   NavbarComp,
    SpinnerComp,
    FooterComp,
    
  },
  data() {

  }
 }
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #f9fbfd;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #f5f6f7;
  
}

nav a.router-link-exact-active {
  border: solid 1px black;
  padding: 5px;
  color: #000000;
  background: white;
  border-radius: 0 20px 20px 0;
  box-shadow: 2px 4px 7px rgb(6, 2, 2);
  transition: transform .6s;
}

nav a.router-link-exact-active:hover {
  transform: scale(0.2); 
}
</style>



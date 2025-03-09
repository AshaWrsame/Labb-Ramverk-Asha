
<script>
import { RouterView } from 'vue-router';
import FooterComp from './components/FooterComp.vue';
import NavBar from './components/NavBar.vue'
export default {
  name: 'App',
  components: {
    NavBar,
    FooterComp,
    RouterView,
  },
data() {
  return {
    currentPage:'home',}
},
watch: {
  $route(to) {
    if (to.path === '/') {
      this.currentPage = 'home';
    } else if (to.path === '/about'){
      this.currentPage = 'about';
    }
  },
  },
};


</script>

<template>
<NavBar :currentPage="currentPage"/>
<RouterView/>
  <FooterComp/>
</template>

<style>

</style>

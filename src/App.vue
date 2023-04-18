<script setup>
  import { RouterView } from 'vue-router'
</script>

<template>
  <NavBar/>
  <RouterView />
  <MainFooter/>
</template>

<script>

  import NavBar from './components/NavBar.vue';
import MainFooter from './components/MainFooter.vue';

  export default{
    components:{
    NavBar,
    MainFooter
}
  }

</script>

<style>

</style>

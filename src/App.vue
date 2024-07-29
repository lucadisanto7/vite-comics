<script>
import 'bootstrap/dist/css/bootstrap.min.css';
import 'bootstrap/dist/js/bootstrap.bundle.min.js';
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
export default {
  components:{
    AppHeader,
    AppMain
  }
}
</script>
<template>
  <div>
    <AppHeader />
    <AppMain />
  </div>
</template>
<style>
  
</style>
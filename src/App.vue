<script>
  //collego i tre file a App
  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';
  import AppFooter from './components/AppFooter.vue';


  export default{
    // Richiamo i file 
    components:{
      AppHeader,
      AppMain,
      AppFooter,  
    }
  }
</script>

<template>
  <!-- Utilizzo i file  -->
  <AppHeader/>
  <AppMain/>
  <AppFooter/>
</template>

<style scoped>

</style>

<script>
  //collego i tre file a App
  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';
  import AppBonus from './components/AppBonus.vue';
  import AppFooter from './components/AppFooter.vue';

  export default{
    // Richiamo i file 
    components:{
      AppHeader,
      AppMain,
      AppBonus,
      AppFooter,
    }
  }
</script>

<template>
    <!-- Utilizzo i file  -->
    <AppHeader/>
    <AppMain/>
    <AppBonus/>
    <AppFooter/>
</template>

<style lang="scss">
  @use './style/generlas.scss' as *;
  @use './style/partials/varibles';
</style>

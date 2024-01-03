<template>
  <HeaderApp />
  <AsideApp />
  <MainApp>
    <CalenderApp />
  </MainApp>
  <FooterApp />
</template>

<script>
import HeaderApp from './components/HeaderApp.vue';
import MainApp from './components/MainApp.vue';
import AsideApp from './components/AsideApp.vue';
import CalenderApp from './components/CalenderApp.vue';
import FooterApp from './components/FooterApp.vue';

export default {
  name: 'App',
  components: {
    HeaderApp,
    MainApp,
    CalenderApp,
    AsideApp,
    FooterApp
  }
}
</script>

<style lang="scss">
@use './components/style/main.scss' as *;
</style>

<!-- 
cd C:\Users\berna\webapp-learn\webapp
npm run dev
-->

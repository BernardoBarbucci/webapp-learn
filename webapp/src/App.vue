<template>
  <HeaderApp />
  <MainApp />
  <FooterApp />
</template>

<script>
import HeaderApp from './components/HeaderApp.vue';
import MainApp from './components/MainApp.vue';
import FooterApp from './components/FooterApp.vue';

export default {
  name: 'App',
  components: {
    HeaderApp,
    MainApp,
    FooterApp
  }
};
</script>

<style lang="scss">
@use './components/style/main.scss' as *;
</style>

<!-- 
cd C:\Users\berna\webapp-learn\webapp
npm run dev
-->

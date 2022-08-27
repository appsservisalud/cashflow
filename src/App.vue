<template>
<Suspense>

  <template #default>
    <Home/>
  </template>

  <template #fallback>
    <SplashScreen/>
  </template>

</Suspense>
</template>

<script>

import SplashScreen from './components/SplashScreen.vue';
import { defineAsyncComponent } from 'vue';

export default {
  name: 'App',
  components: {
    SplashScreen,
    Home: defineAsyncComponent(() => {
      return new Promise((resolve) => {
        setTimeout(() => {
          resolve(require("./components/Home.vue"));
        }, 2500);
      });
    })
  
}}

</script>


<style>
@import './assets/css/App/app.css';
</style>





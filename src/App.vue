<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  components: {AppHeader, AppMain, AppFooter},
}

</script>

<template>
  <app-header></app-header>
  <app-main></app-main>
  <app-footer></app-footer>
</template>

<style>
  body {
    font-family: 'Poppins', sans-serif;
  }

/* GENERICS  */

ul {
  list-style-type: none;
  padding: 0 !important;
}

ul li a {
  text-decoration: none;
}



</style>
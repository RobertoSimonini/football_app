<script>
import Navbar from './components/Navbar.vue';
import Jumbotron from './components/Jumbotron.vue';
import AppMain from './components/AppMain.vue';
import BigMatch from './components/BigMatch.vue';
import UpcomingMatch from './components/UpComingMatch.vue';
import PlayerSection from './components/PlayerSection.vue';
import LeagueTable from './components/LeagueTable.vue';
import Results from './components/Results.vue';
import NewsSection from './components/NewsSection.vue';
import NewsCard from './components/NewsCard.vue';
import AppSponsor from './components/AppSponsor.vue';
import AppFooter from './components/AppFooter.vue';
import { store } from './store';

export default {
  components: {Navbar, Jumbotron, BigMatch, UpcomingMatch, LeagueTable, Results, NewsSection, NewsCard, AppMain, PlayerSection, AppSponsor, AppFooter},
  data() {
    return {
      store,

    }
  }
}

</script>

<template>
  <Jumbotron></Jumbotron>
  <big-match></big-match>
  <upcoming-match></upcoming-match>
  <player-section></player-section>
  <league-table></league-table>
  <app-sponsor></app-sponsor>
  <news-section></news-section>
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
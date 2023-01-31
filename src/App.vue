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
import AppFooter from './components/Appfooter.vue';

import { store } from './store';

export default {
  components: {Navbar, Jumbotron, BigMatch, UpcomingMatch, LeagueTable, Results, NewsSection, NewsCard, AppFooter, AppMain, PlayerSection },
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
</template>

<style>

</style>
<script>
import BigMatch from './BigMatch.vue';
import UpComingMatch from './UpComingMatch.vue';
import PlayerSection from './PlayerSection.vue';
import LeagueTable from './LeagueTable.vue';
import AppSponsor from './AppSponsor.vue';
import NewsSection from './NewsSection.vue';
export default {
    components: {BigMatch, UpComingMatch, PlayerSection, LeagueTable, AppSponsor, NewsSection}
}

</script>

<template>
<big-match></big-match>
<UpComingMatch></UpComingMatch>
<player-section></player-section>
<league-table></league-table>
<app-sponsor></app-sponsor>
<news-section></news-section>

</template>


<style scoped>

</style>
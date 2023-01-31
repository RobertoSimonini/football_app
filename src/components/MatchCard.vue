<script>
export default {
    props: {
        match: Object
    }
}
</script>


<template>
    <!-- Qui metto l'intere informazioni relative al singolo match  -->

    <div class="match-container d-flex flex-column text-white align-items-center justify-content-center my-3">

        <!-- Qui metto solo le squadre -->
        <div class="teams d-flex align-items-center">
            <div class="home-team d-flex align-items-center">
                <img :src="match.homePic" alt="">
                <h2> {{ match.homeTeam }}</h2>
            </div>

                <h1 class="px-3"> VS </h1>

            <div class="transfer-team d-flex align-items-center">
                <h2> {{ match.transferTeam }} </h2>
                <img :src="`${match.transferPic}`" alt="">
            </div>
        </div>

        <!-- Qui metto la data e lo stadio dove si giocherà la partita  -->
        <div class="other-info w-100">
            <div class="date d-flex justify-content-center align-items-center fw-bold">
                <i class="fa-solid fa-calendar-days text-secondary pe-1"></i>
                <span class="pe-3"> {{match.date}} </span>

                <i class="fa-solid fa-circle-plus text-secondary pe-1"></i>
                <span> {{ match.stadium }} </span>
            </div>
        </div>
    </div>

</template>



<style scoped>

</style>
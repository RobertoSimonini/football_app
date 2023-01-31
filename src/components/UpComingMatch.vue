<script>
export default {
    
}

</script>

<template>

<section id="upcoming-matches" class="text-center py-5 px-4">

    <h2 class="text-white">
        Upcoming Matches
    </h2>

    <!-- Qui metto l'intere informazioni relative al singolo match  -->
    <div class="match-container d-flex flex-column text-white align-items-center justify-content-center my-3">

        <!-- Qui metto solo le squadre -->
        <div class="teams d-flex align-items-center">
            <div class="home-team d-flex align-items-center">
                <img src="../assets/img/league-club-3.png" alt="">
                <h2>Istanbul Sport</h2>
            </div>
    
                <h1 class="px-3"> VS </h1>
    
            <div class="transfer-team d-flex align-items-center">
                <h2>United Fs Club </h2>
                <img src="../assets/img/league-club-4.png" alt="">
            </div>
        </div>

        <!-- Qui metto la data e lo stadio dove si giocherà la partita  -->
        <div class="other-info w-100">
            <div class="date d-flex justify-content-center align-items-center fw-bold">
                <i class="fa-solid fa-calendar-days text-secondary pe-1"></i>
                <span class="pe-3"> May 21, 2022 18:05 pm </span>

                <i class="fa-solid fa-circle-plus text-secondary pe-1"></i>
                <span>Expert Stadium </span>
            </div>
        </div>
    </div>

</section>

</template>


<style lang="scss" scoped>
    #upcoming-matches {
        height: 1000px;
        background-image: url(../assets/img/saha.jpg);
        background-position: center;
        background-size: cover;
        background-repeat: no-repeat;

        .match-container {
            background-color: rgb(16 29 47 / 50%);

            .other-info {
                background-color: rgb(14 18 23 / 50%);
            }
        }
    }


</style>
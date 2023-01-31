<script>
export default {

}

</script>


<template>

    <section id="next-match" class="d-flex flex-column align-items-center justify-content-center">
        <!-- Qui metto la partita in primo piano  -->
        <div class="d-flex align-items-center justify-content-center">
            <div class="home-team d-flex align-items-center">
                <h2>Istanbul Sport</h2>
                <img src="../assets/img/league-club-1.png" alt="">
            </div>

            <h1 class="px-3"> VS </h1>

            <div class="transfer-team d-flex align-items-center">
                <img src="../assets/img/league-club-2.png" alt="">
                <h2>United Fs Club </h2>
            </div>
        </div>

        <!-- Qui metto la data della partita  -->
        <div class="date d-flex justify-content-center align-items-center fw-bold">
            <i class="fa-solid fa-calendar-days text-secondary pe-1"></i>
            <span class="pe-3"> May 21, 2022 18:05 pm </span>

            <i class="fa-solid fa-circle-plus text-secondary pe-1"></i>
            <span>Expert Stadium </span>
        </div>

            <a href="#" class="btn btn-dark my-3">View Match details </a>

    </section>


</template>





<style scoped>

    #next-match {
        height: 300px;

    }

    a {
        padding: 20px 40px;
        font-size: 20px;
        border-radius: 30px;
    }

</style>
<script>
export default {
    
}

</script>

<template>
    <section id="news" class="p-4">
        <!-- Qui metto lo slogan promozionale della sezione News  -->
        <div class="news-top text-center">
            <figure>
                <img src="../assets/img/like_button.png" alt="">
                <figcaption>
                    <h1>Recent News & Articles</h1>
                    <article class="fw-light">Be aware of the football world.</article>
                </figcaption>
            </figure>
        </div>

        <!-- Qui inserisco le card riferite alle News  -->
        <div class="news-bottom container d-flex">
            <div class="row g-3 justify-content-center">
                <div class="col-3">
                    <!-- Qui metto la card che parla di cosa è il calcio  -->
                    <div class="card">
                        <img src="../assets/img/news1-1-150x150.png" class="card-img-top" alt="...">
                        <div class="card-body text-center">
                            <p class="fw-bold">29.05.2022 - Football</p>
                            <h5 class="card-title">What is Football?</h5>
                            <p class="card-text">Football is a sport that is known as a ball game and is loved by [...].</p>
                            <a href="#" class="btn btn-dark"> More </a>
                        </div>
                    </div>
                </div>

                <!-- QUi metto la card che parla delle regole del calcio  -->
                <div class="col-3">
                    <div class="card">
                        <img src="../assets/img/news3-1-150x150.png" class="card-img-top" alt="...">
                        <div class="card-body text-center">
                            <p class="fw-bold">29.05.2022 - Football</p>
                            <h5 class="card-title">Football Rules</h5>
                            <p class="card-text">GOLDEN GOAL: in a football match, the goal scored by one of the items (this rule doesn't exist anymore) [...]</p>
                            <a href="#" class="btn btn-dark"> More </a>
                        </div>
                    </div>
                </div>
                
                <!-- Qui metto la card che parla delle novità del calcio  -->
                <div class="col-3">
                    <div class="card">
                        <img src="../assets/img/news6-1-150x150.png" class="card-img-top" alt="...">
                        <div class="card-body text-center">
                            <p class="fw-bold">29.05.2022 - Football</p>
                            <h5 class="card-title">Football Feautures</h5>
                            <p class="card-text"> Football: it is an anaerobic-based anaerobic sport in which jumps, in which kicks, turns, running with changing the direction you're running can make the defenders miss the tackle and it may be  [...] </p>
                            <a href="#" class="btn btn-dark"> More </a>
                        </div>
                    </div>
                </div>
                <!-- Qui metto la card che parla dei terms del calcio  -->
                <div class="col-3">
                    <div class="card">
                        <img src="../assets/img/news4-1-150x150.png" class="card-img-top" alt="...">
                        <div class="card-body text-center">
                            <p class="fw-bold">29.05.2022 - Football</p>
                            <h5 class="card-title">Football Terms</h5>
                            <p class="card-text"> GOLDEN GOAL: in a football match, the goal scored by one of the items (this rule doesn't exist anymore) [...] </p>
                            <a href="#" class="btn btn-dark"> More </a>
                        </div>
                    </div>
                </div>
            </div>
        
        </div>
    </section>

</template>


<style scoped>
    .news-top figure img {
        height: 200px;
    }

    .card {
        padding: 25px;
        border: none;
        box-shadow: 0 0 5px gray;
    }

    a {
    padding: 20px 40px;
    font-size: 20px;
    border: 1px solid #fff;
    border-radius: 30px;
    }

</style>
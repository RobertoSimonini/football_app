<script>
export default {
    data (){
        return {
            players: [
                        {
                            pic: '/src/assets/img/player1.jpg',
                            number: '07',
                            name: 'Adam Brown -',
                            role: 'Forwarder'
                        },
                        {
                            pic: '/src/assets/img/player2.jpg',
                            number: '09',
                            name: 'Michael Kayn -',
                            role: 'Forwarder'
                        },
                        {
                            pic: '/src/assets/img/player3.jpg',
                            number: '11',
                            name: 'Michelle Lee -',
                            role: 'Forwarder'
                        },
                        {
                            pic: '/src/assets/img/player4.jpg',
                            number: '15',
                            name: 'Ethan Smith -',
                            role: 'Midfielder'
                        },
            ]
        }
    }
}
</script>


<template>

    <section id="players" class="text-center py-5 px-4 text-white d-flex flex-column align-items-center justify-content-between">
        <h2>
            Players
        </h2>
        <div class="container-fluid">

            <div class="row g-5">
                <div class="col-3" v-for="player in players">
                    <div class="product-card text-center">
                        <figure>
                            <img :src="player.pic" class="img-fluid h-100 w-100" alt="...">
                            <figcaption class="d-flex flex-column justify-content-center">
                                <div class="number fw-bold">
                                    {{ player.number }}
                                </div>
                                <div class="name">
                                    <h4>
                                        {{player.name}} 
                                    </h4>
                                    <h4>
                                        {{player.role}}
                                    </h4>
                                </div>
                            </figcaption>
                        </figure>

                    </div>
                </div>
            </div>

            
        </div>

        <a href="#" class="btn btn-dark my-3">View All Players </a>

    </section>

</template>


<style lang="scss" scoped>

    #players {
        height: 750px;
        background-image: url(../assets/img/player.jpg);
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
    }

.product-card {
    height: 450px;
    width: 400px;
    padding: 0;
    border: none;
    position: relative;
    cursor: pointer;
}

figure {
    height: 100%;

    img {
        border-radius: 25px;
    }

    figcaption {
        position: absolute;
        bottom: 0;
        left: 0;
        right: 0;
        height: 125px;
        padding: 0 75px;

        background-color: black;
        border-radius: 25px;

        .number {
            font-size: 25px;
        }

        .name h4 {
            color: #B3B3B3;
        }
    }
}


a {
    padding: 20px 40px;
    font-size: 20px;
    border: 1px solid #fff;
    border-radius: 30px;
}

</style>
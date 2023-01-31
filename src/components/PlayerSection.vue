<script>
import PlayerCard from './PlayerCard.vue';
export default {
    components: {PlayerCard},
    data (){
        return {
            players: [
                        {
                            pic: '/src/assets/img/player1.jpg',
                            number: '07',
                            name: 'Adam Brown -',
                            role: 'Forwarder',
                            id: 1
                        },
                        {
                            pic: '/src/assets/img/player2.jpg',
                            number: '09',
                            name: 'Michael Kayn -',
                            role: 'Forwarder',
                            id: 2
                        },
                        {
                            pic: '/src/assets/img/player3.jpg',
                            number: '11',
                            name: 'Michelle Lee -',
                            role: 'Forwarder',
                            id: 2
                        },
                        {
                            pic: '/src/assets/img/player4.jpg',
                            number: '15',
                            name: 'Ethan Smith -',
                            role: 'Midfielder',
                            id: 3
                        },
            ]
        }
    },
    
}
</script>


<template>

    <section id="players" class="text-center py-5 px-4 text-white d-flex flex-column align-items-center justify-content-between">
        <h2>
            Players
        </h2>
        <div class="container-fluid">

            <div class="row g-5">
                <player-card v-for="player in players" :player="player" :key="player.id"></player-card>   
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

a {
    padding: 20px 40px;
    font-size: 20px;
    border: 1px solid #fff;
    border-radius: 30px;
}


</style>
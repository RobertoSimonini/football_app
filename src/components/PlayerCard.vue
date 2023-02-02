<script>
export default {
    props: {player: Object}
}

</script>

<template>
    <div class="col-3">
        <div class="player-card text-center">
            <figure>
                <img :src="player.pic" class="img-fluid h-100 w-100" :alt="player.name">
                <figcaption class="d-flex flex-column justify-content-center py-2">
                    <div class="number fw-bold">
                        {{ player.number }}
                    </div>
                     <div class="name">
                        <h5>
                            {{player.name}} 
                        </h5>
                        <h5>
                            {{player.role}}
                        </h5>
                    </div>
                </figcaption>
            </figure>

        </div>
    </div>

</template>

<style lang="scss" scoped>
.player-card {
    height: 375px;
    width: 300px;
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



</style>
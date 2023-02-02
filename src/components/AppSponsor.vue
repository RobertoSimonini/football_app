<script>
export default {
    data(){
        return {
            sponsors: [
                {
                    url: '/src/assets/img/client2.png',
                    id: 1
                },
                {
                    url: '/src/assets/img/client3.png',
                    id: 2
                },
                {
                    url: '/src/assets/img/client4.png',
                    id: 3
                },
                {
                    url: '/src/assets/img/client7.png',
                    id: 4
                },
                {
                    url: '/src/assets/img/client9.png',
                    id: 1
                },
                {
                    url: '/src/assets/img/client10.png',
                    id: 1
                },
            ]
        }
    }
}

</script>


<template>
        <section id="sponsor">
            <div class="sponsor-top">
                <figure class="h-100">
                    <img class="h-100" src="../assets/img/reklam.jpg" alt="">
                </figure>
            </div>
            <div class="sponsor-bottom d-flex justify-content-between align-items-center px-5">
                <figure v-for="sponsor in sponsors" :key="sponsor.id">
                    <img role="button" :src="sponsor.url" alt="">
                </figure>
            </div>  
        </section>

</template>







<style lang="scss" scoped>
    #sponsor {
        min-height: 300px;

        .sponsor-top {
            height: 275px;
            img {
                object-fit: cover;
                height: 100%;
                width: 100%;
            }
        }

        .sponsor-bottom {
            height: 275px;
            background-color: #9b51e0;
            color: #fff;

            img {
                height: 200px;
                border: 2px solid #ffff;
                padding: 1.5rem;
                border-radius: 50px;
            }

        }
    }
</style>
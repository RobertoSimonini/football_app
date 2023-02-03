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
                    id: 5
                },
                {
                    url: '/src/assets/img/client10.png',
                    id: 6
                },
            ]
        }
    }
}

</script>


<template>

        <section id="sponsor">
            <div class="container">
                <!-- Slogan  -->
                <div class="sponsor-top">
                    <figure class="h-100">
                        <img class="h-100" src="../assets/img/reklam.jpg" alt="">
                    </figure>
                </div>
            </div>

            <!-- Aziende sponsors  -->
            <div class="sponsor-bottom">
                <div class="container d-flex justify-content-between align-items-center px-5 h-100">
                    <figure v-for="sponsor in sponsors" :key="sponsor.id">
                        <img role="button" :src="sponsor.url" alt="">
                    </figure>
                </div>
            </div>  
        </section>

</template>







<style lang="scss" scoped>
    #sponsor {
        .sponsor-top {
            img {
                object-fit: cover;
                object-position: center;
                width: 100%;
            }
        }

        .sponsor-bottom {
            height: 275px;
            background-color: #9b51e0;
            color: #fff;

            img {
                height: 150px;
                border: 2px solid #ffff;
                padding: 1.5rem;
                border-radius: 50px;
                transition: transform 0.25s;

                &:hover {
                    transform: scale(1.05);
                }
            }

        }
    }
</style>
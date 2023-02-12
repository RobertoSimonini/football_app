<script>
import Navbar from './AppNavbar.vue';
export default {
    components: {Navbar},
    data(){
        return {
            currentIndex: 0,
            autoPlaySupport: null,
            pictures: [
                    {
                    url: '/src/assets/img/slider1-1.jpg',
                    id: 0
                },
                {
                    url: '/src/assets/img/slider2-1.jpg',
                    id: 1
                },
                {
                    url: '/src/assets/img/slider3.jpg',
                    id: 2
                },
                {
                    url: '/src/assets/img/slider4.jpg',
                    id: 3
                },
            ]
        }
    },

    computed: {
        prevInfinite() {
            if (this.currentIndex < 0) {
                return this.currentIndex = this.pictures.length - 1;
            }
        },
        
        nextInfinite() {
            if (this.currentIndex === this.pictures.length) {
                return this.currentIndex = 0;
            }
        }
    },
    
    methods: {
        changeThumb(index) {
        this.currentIndex = index;
        },
        
        autoPlay(){
            this.autoPlaySupport = setInterval (() =>{
                this.currentIndex++
                this.nextInfinite(); 
            }, 3000);   
        },

        stopAutoPlay(){
            clearInterval(this.autoPlaySupport);
        },
    },


    mounted () {
        this.autoPlay()
    }
     
} 


</script>


<template>

<section id="jumbotron">
    <Navbar></Navbar>
    <img @mouseover="stopAutoPlay" v-for="pic in pictures" class="img-fluid" :src="pic.url" alt="" v-show="currentIndex === pic.id" :key="pic.id">
    
    <div class="prev">
        <i @click="currentIndex--, prevInfinite" class="fa-solid fa-circle-chevron-left"></i>
    </div>

    <div class="next">
        <i @click="currentIndex++, nextInfinite" class="fa-solid fa-circle-chevron-right"></i>
    </div>


    <div class="content text-center text-white position-absolute z-1">
        <div>
            <h1>
                FootBall Club
            </h1>
            <h1>
                Sport Club
            </h1>
        </div>
        <h3>
            Private Football matches
        </h3>
        <a class="btn btn-outline-light" href="#">Learn More <i class="fa-solid fa-arrow-right"></i> </a>
    </div>


</section>

</template>




<style lang="scss" scoped>

#jumbotron {

    position: relative;
    height: 750px;

    img {
        object-fit: cover;
        object-position: bottom;
        height: 100%;
        width: 100%;
    }

    img.active {
        display: block;
    }

}
.content {
    top: 60%;
    left: 50%;
    transform: translate(-50%, -60%);

    h1 {
        font-size: 75px;
    }        

    a {
        padding: 20px 40px;
        font-size: 20px;
        border-radius: 30px;
    }

    > * {
        margin: 1.5rem 0;
    }
}

.prev, .next {
    position: absolute;
    top: 50%;
    font-size: 50px;
    z-index: 1;
    color: white;
    cursor: pointer;
}

.prev {
    left: 2rem;
}

.next {
    right: 2rem;
}




</style>
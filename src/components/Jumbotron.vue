<script>
import Navbar from './Navbar.vue';
export default {

    components: {Navbar}

}

</script>


<template>

<section id="jumbotron">
    <Navbar></Navbar>
    <img class="img-fluid" src="../assets/img/slider2-1.jpg" alt="">
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
}

</style>
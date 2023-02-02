<script>
export default {
    
}
</script>

<template>
    <footer class="p-3">
        <div class="row">
            <div class="col-2 infos">
                <ul>
                    <li>
                        <img src="../assets/img/logo-football.png" alt="">
                    </li>
                    <li>
                        <i class="fa-solid fa-location-dot"></i>
                        <span> New Jersey, USA</span>
                    </li>
                    <li>
                        <i class="fa-solid fa-phone-volume"></i>
                        <span> +1 (234) 567 89 10</span>
                    </li>

                    <li>
                        <i class="fa-solid fa-envelope"></i>
                        <span> example@example.com </span>
                    </li>

                    <li class="socials">
                        <i class="fa-brands fa-facebook-f"></i>
                        <i class="fa-brands fa-instagram"></i>
                        <i class="fa-brands fa-twitter"></i>
                    </li>
                    
                </ul>
            </div>

            <div class="col-6">

            </div>

            <div class="col-2">

            </div>

            <div class="col-2">

            </div>

        </div>
    </footer>
</template>


<style lang="scss" scoped>
   footer {
    height: 500px;
    background-color: #000000;
    color: #ffff;

    ul {
        list-style-type: none;
    }
   }

   .infos > ul li{
        padding: 1rem 0.25rem;
        
        img {
            height: 100px;
            filter: grayscale(1);
        }

    }
    .socials i{
        font-size: 35px;
        margin-right: 1rem;
        padding: 0.25rem 0.5rem;
        border: 1px solid #ffff;
    }

</style>    
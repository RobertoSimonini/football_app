<script>
export default {
    
}
</script>

<template>
    <footer class="p-3">
        <div class="row justify-content-between">
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

            <div class="col-4 newsletter">
                <h1>Join our New Newsletter</h1>
                <p>
                    Subscribe to be informed about important development in our club and football world,
                </p>

                <div class="input-group mb-3">
                    <input type="text" class="form-control w-100" placeholder="Your email adress">
                    <button type="button" class="btn btn-outline-light w-100 my-3">Subscribe -></button>
                </div>
            </div>

            <div class="col-2 education">
                <h2>
                    Education
                </h2>
                
                <ul>
                    <li>
                        <a href="#">- FIXTURES AND RESULTS</a>
                    </li>
                    <li>
                        <a href="#">- LEAGUE TABLE</a>
                    </li>
                    <li>
                        <a href="#">- PLAYERS </a>
                    </li>
                    <li>
                        <a href="#">- GALLERY </a>
                    </li>
                </ul>
            </div>

            <div class="col-2 lins">
                <h2>
                    Quick Lins
                </h2>
                <ul>
                    <li>
                        <a href="#">- HOME</a>
                    </li>
                    <li>
                        <a href="#">- BLOG </a>
                    </li>
                    <li>
                        <a href="#">- GALLERY </a>
                    </li>
                    <li>
                        <a href="#">- CONTACT </a>
                    </li>
                </ul>
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

//    Qui metto le infos 
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


// QUi metto la la newsletter 
.newsletter input, button {
    padding: 1.5rem 2rem;
    border-radius: 2.25rem !important;
    background-color: #fff;
    color: #000000;
}

// Qui metto la col dell'education 

.education, .lins ul{
    li a {
        color: #ffff;
        font-size: 17.5px;
        line-height: 40px;
        padding: 0;
    }
}


</style>    
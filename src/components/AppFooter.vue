<script>
export default {
    data (){
        return {
            email: '',
            emails: []
            }
    },
    methods: {
        subEmail (){
            this.emails.push(this.email);
            this.email = '';
        }
    }
}
</script>

<template>
    <footer class="px-3 py-5">
        <div class="container">
            <div class="row justify-content-around">
                <div class="col-3 infos">
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
                        <input v-model="email" type="email" class="form-control w-100" placeholder="Your email adress">
                        <button @click="subEmail" type="button" class="btn btn-outline-light w-100 my-3">Subscribe <i class="fa-solid fa-arrow-right"></i></button>
                    </div>
                </div>
    
                <div class="col-2 education">
                    <h2>
                        Education
                    </h2>
                    
                    <ul>
                        <li>
                            <a href="#"><i class="fa-solid fa-minus"></i> FIXTURES AND RESULTS</a>
                        </li>
                        <li>
                            <a href="#"> <i class="fa-solid fa-minus"></i> LEAGUE TABLE</a>
                        </li>
                        <li>
                            <a href="#"><i class="fa-solid fa-minus"></i> PLAYERS </a>
                        </li>
                        <li>
                            <a href="#"><i class="fa-solid fa-minus"></i> GALLERY </a>
                        </li>
                    </ul>
                </div>
    
                <div class="col-2 lins">
                    <h2>
                        Quick Lins
                    </h2>
                    <ul>
                        <li>
                            <a href="#"><i class="fa-solid fa-minus"></i> HOME</a>
                        </li>
                        <li>
                            <a href="#"><i class="fa-solid fa-minus"></i> BLOG </a>
                        </li>
                        <li>
                            <a href="#"><i class="fa-solid fa-minus"></i> GALLERY </a>
                        </li>
                        <li>
                            <a href="#"><i class="fa-solid fa-minus"></i> CONTACT </a>
                        </li>
                    </ul>
                </div>
    
                <div class="col-12 text-center">
                    2022 Football Club. <i class="fa-solid fa-minus"></i> All Rights reserved.
                </div>
    
            </div>
        </div>
    </footer>
</template>


<style lang="scss" scoped>
   footer {
    background-color: #9b51e0;
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
        font-size: 25px;
        margin-right: 1rem;
        padding: 0.25rem 0.5rem;
        border: 1px solid #ffff;
        cursor: pointer;
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
        font-size: 15px;
        line-height: 40px;
        padding: 0;
    }
}


</style>    
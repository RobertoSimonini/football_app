<script>
export default {
    data(){
        return {
            links: [
                {
                    text: 'Home',
                    href: '#'
                },
                {
                    text: 'Fixtures & Results',
                    href: '#'
                },
                {
                    text: 'League Table',
                    href: '#'
                },
                {
                    text: 'Players',
                    href: '#'
                },
                {
                    text: 'Gallery',
                    href: '#'
                },
                {
                    text: 'Blog',
                    href: '#'
                },
                {
                    text: 'Contact',
                    href: '#'
                }
            ]
        }
    }
}

</script>


<template>

<nav>
    
    
    <!-- Qui metto il Logo in position absolute rispetto alla Nav  -->
    <figure id="logo">
        <img src="../assets/img/logo-football.png" alt="">
    </figure> 
    
    <!-- Qui metto la parte riferita agli sponsor e ai social  -->
    <div class="nav-top d-flex justify-content-center h-50 z-1 position-relative">


        <!-- Qui metto gli sponsor  -->
        <div class="sponsors h-100">
            <ul class="h-100">
                <li>
                    <a href="#">
                        <img src="../assets/img/sponsor1.png" alt="">
                    </a>
                </li>
    
                <li>
                    <a href="#">
                        <img src="../assets/img/sponsor2.png" alt="">
                    </a>
                </li>
            </ul>
        </div>

        <!-- Qui metto i social  -->
        <div class="social h-100">
            <ul class="h-100">
                <li>
                    <a href="#">
                        <i class="fa-brands fa-facebook-f fa-xl"></i>
                    </a>
                    <a href="#">
                        <i class="fa-brands fa-instagram fa-xl"></i>
                    </a>
                    <a href="#">
                        <i class="fa-brands fa-twitter fa-xl"></i>
                    </a>
                </li>
            </ul>
        </div>  
        


    </div>
    <!-- Qui metto la parte riferita alla parte di navigazione  -->
    <div class="nav-bottom h-50">
        <ul class="h-100">
            <li v-for="link in links">
                <a :href="link.href" class="fw-bold px-5">
                    {{ link.text }}
                </a>
            </li>
        </ul>
    </div>
</nav>

</template>



<style lang="scss" scoped>

    nav {
        height: 200px;
        background-color: rgb(2,7,10, 0.5);
        position: absolute;
        top: 0;
        right: 0;
        left: 0;

        ul {
            list-style-type: none;
            display: flex;
            justify-content: center;
            align-items: center;

            li a {
                color: white;
                text-decoration: none;
                text-transform: uppercase;
            }
        }
    }

    .sponsors {

        transform: translateX(-50px);

        a {
            padding: 0 10px;
        }
    }

    .social {
        a {
            font-size: 22.5px;
            padding: 0 0.5rem;
        }
    }

    #logo {
        position: absolute;
        top: 10px;
        left: 50%;
        transform: translateX(-50%);

    }

</style>
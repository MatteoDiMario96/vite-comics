<script>
export default {
    data() {
        return {
            
        }
    },
    methods:{

    },
    created(){

    }
}
</script>


<template>
    <footer>
        <section id="ul-links">
            
        </section>

        <nav>
            <button>
                Signup-Now
            </button>

            <section id="sign-up-social">
            <div id="follow_us">
                <h2>
                Follow us
                </h2>
            </div>
            <div id="favicon">
                <a href="#">
                    <i class="fa-brands fa-facebook fa-xl"></i>
                    *
                </a>
                <a href="#">
                    <i class="fa-brands fa-twitter"></i>
                    *
                </a>
                <a href="#">
                    <i class="fa-brands fa-youtube"></i>
                    *
                </a>
                <a href="#">
                    <i class="fa-brands fa-pinterest-p"></i>
                    *
                </a>
                <a href="#">
                    <i class="fa-brands fa-google"></i>
                    *
                </a>
            </div>
        </section>
        </nav>
        
    </footer>
</template>

<style lang="scss" scoped>
        nav{
            display: flex;
            justify-content: space-between;
            align-items: center;
            background-color: #303030;
            height: 70px;
            padding: 1rem;
            button{
                background-color: #303030;
                border: 2px solid #0777df;
                color: white;
                padding: .6rem;
                text-transform: uppercase;
                font-weight: 600;
            }
            section#sign-up-social{
                display: flex;
                align-items: center;
                padding: 1rem;
                div{
                    h2{
                        color:#0777df;
                    }
                    padding: 1rem;
                    a{
                        padding: .3rem;
                    }
                }
            }
        }
        


</style>
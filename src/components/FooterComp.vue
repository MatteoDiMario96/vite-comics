<script>
export default {
    data() {
        return {
            FooterUlLinksDCComics: [
                {
                    id: 1,
                    title: 'Characters',
                    href: '#',
                },{
                    id: 2,
                    title: 'Comics',
                    href: '#',
                },{
                    id: 3,
                    title: 'Movies',
                    href: '#',
                },{
                    id: 4,
                    title: 'Tv',
                    href: '#',
                },{
                    id: 5,
                    title: 'Games',
                    href: '#',
                },{
                    id: 6,
                    title: 'Videos',
                    href: '#',
                },{
                    id: 7,
                    title: 'News',
                    href: '#',
                },
            ],
            FooterUlLinksShop: [
                {
                    id: 1,
                    title: 'Shop DC',
                    href: '#',
                },{
                    id: 2,
                    title: 'Shop DC Collectibles',
                    href: '#',
                },
            ],
            FooterUlLinksDC: [
                {
                    id: 1,
                    title: 'Term of use',
                    href: '#',
                },{
                    id: 2,
                    title: 'Privacy policy(New)',  
                    href: '#',           
                },{
                    id: 3,
                    title: 'Ad Choices',
                    href: '#',
                },{
                    id: 4,
                    title: 'Advertising',
                    href: '#',
                },{
                    id: 5,
                    title: 'Jobs',
                    href: '#',
                },{
                    id: 6,
                    title: 'Subscriptions',
                    href: '#',
                },{
                    id: 7,
                    title: 'Talent Workshops',
                    href: '#',
                },{
                    id: 8,
                    title: 'CPSC Certificates',
                    href: '#',
                },{
                    id: 9,
                    title: 'Ratings',
                    href: '#',
                },{
                    id: 10,
                    title: 'Shop help',
                    href: '#',
                },{
                    id: 11,
                    title: 'Contact Us',
                    href: '#',
                },
            ],
            FooterUlLinksSites: [
                {
                    id: 1,
                    title: 'DC',
                    href: '#',
                },{
                    id: 2,
                    title: 'MAD Magazine',
                    href: '#',
                },{
                    id: 3,
                    title: 'DC Kids',
                    href: '#',
                },{
                    id: 4,
                    title: 'DC Universe',
                    href: '#',
                },{
                    id: 5,
                    title: 'DC Power Visa',
                    href: '#',
                },
            ],
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
            <div id="ul">
                <div>
                    <ul id="dc_comics">
                    <h2>
                        Dc Comics
                    </h2>
                    <li v-for="link in FooterUlLinksDCComics" :key="link.id">
                        <a :href="link.href">
                            {{ link.title }}
                        </a>
                    </li>
                </ul>
                
                <ul id="shop">
                    <h2>
                        Shop
                    </h2>
                    <li v-for="link in FooterUlLinksShop" :key="link.id">
                        <a :href="link.href">
                            {{ link.title }}
                        </a>
                    </li>
                </ul>
                
                </div>
                
                <ul id="dc">
                    <h2>
                        Dc 
                    </h2>
                    <li v-for="link in FooterUlLinksDC" :key="link.id">
                        <a :href="link.href">
                            {{ link.title }}
                        </a>
                    </li>
                </ul>
                <ul id="sites">
                    <h2>
                        Sites
                    </h2>
                    <li v-for="link in FooterUlLinksSites" :key="link.id">
                        <a :href="link.href">
                            {{ link.title }}
                        </a>
                    </li>
                </ul>
            </div>
            <div id="img">
                
            </div>
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
                    <img src="../assets/img2/footer-facebook.png" alt="Facebook link">
                </a>
                <a href="#">
                    <img src="../assets/img2/footer-twitter.png" alt="Twitter link">
                </a>
                <a href="#">
                    <img src="../assets/img2/footer-youtube.png" alt="YouTube link">
                </a>
                <a href="#">
                    <img src="../assets/img2/footer-pinterest.png" alt="Pinterest link">
                </a>
                <a href="#">
                    <img src="../assets/img2/footer-periscope.png" alt="Periscope link">
                </a>
            </div>
        </section>
        </nav>
        
    </footer>
</template>

<style lang="scss" scoped>
        section#ul-links{
            background-image: url('../assets/img2/footer-bg.jpg');
            padding: 0 0 0 1rem;
            display: flex;
            justify-content: space-between;
            div#ul{
                display: flex;
                flex-direction: row;
                ul{
                    padding-top: 2rem;
                    margin-bottom: 2rem;
                    #shop{
                        padding-top: 1rem;
                    }
                    h2{
                    padding: .3rem;
                    margin-bottom: .3rem;
                    text-transform: uppercase;
                    font-size: 1.15rem;
                    font-weight: 700;
                    color: white;
                    }
                    li{
                        padding: .3rem;
                        font-size: .8rem;                       
                    }
                }
            }
            div#img{
                width: 55%;
                background-image: url('../assets/img2/dc-logo-bg.png');
                background-repeat: no-repeat;
                background-position: left;
            }          
        }
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
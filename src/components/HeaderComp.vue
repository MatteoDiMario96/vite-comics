<script>
export default {
    data() {
        return {
            UlHeaderLinks: [
                {   
                    id: 1,
                    title: "CHARACTERS",
                    active: false,
                    href: "#",
                },{ 
                    id: 2,
                    title: "COMICS",
                    active: true,
                    href: "#",
                },{ 
                    id: 3,
                    title: "MOVIES",
                    active: false,
                    href: "#",
                },{ 
                },{ 
                    id: 4,
                    title: "TV",
                    active: false,
                    href: "#",
                },{ 
                },{ 
                    id: 5,
                    title: "GAMES",
                    active: false,
                    href: "#",
                },{ 
                },{ 
                    id: 6,
                    title: "COLLECTIBLES",
                    active: false,
                    href: "#",
                },{ 
                },{ 
                    id: 7,
                    title: "VIDEOS",
                    active: false,
                    href: "#",
                },{ 
                },{ 
                    id: 8,
                    title: "FANS",
                    active: false,
                    href: "#",
                },{ 
                },{ 
                    id: 9,
                    title: "NEWS",
                    active: false,
                    href: "#",
                },{ 
                },{ 
                    id: 10,
                    title: "SHOP",
                    active: false,
                    href: "#",
                },
            ],
            MainLogo:{
                src: './src/assets/img2/dc-logo.png',
                href: '#',
                alt: "Main logo Dc Comics",
            }
        }
    },
    methods:{

    },
    created(){

    }
}
</script>

<template>
    <header>
        <nav>
            <div id="div-logo">
                <a :href="MainLogo.href">
                    <img :src="MainLogo.src" :alt="MainLogo.alt" id="img-logo">
                </a>
            </div>

            <div id="ul-header">
                <ul>
                    <li v-for="link in UlHeaderLinks" :key="link.id">
                        <a :href="link.href" :class="(link.active === true) ? 'active' : ''">
                            {{ link.title }}
                        </a>
                    </li>
                </ul>
            </div>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;

    header{
        height: 70px;
        padding: 1rem;
        nav{
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 100%;
            #div-logo{
                height: 100%;
                a{
                    height: 100%;
                    img{
                    height: 100%;
                    }
                }
                
            }
            #ul-header{
                ul{
                    display: flex;
                        li{
                            padding: .5rem;
                            a{
                            color: $secondary-color;
                            font-size: .8rem;
                            &.active{
                            color: $primary_color;
                            padding-bottom: 2.3rem;
                            border-bottom: 5px solid $primary_color;
                            }
                        }
                    }
                }
            }
        }
    }
</style>
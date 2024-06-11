
<script>
export default {
    data() {
        return {
            ArticleImgLinks:[
                {
                    id: 1,
                    title: 'Digital Comics',
                    src: './src/assets/img2/buy-comics-digital-comics.png',
                    alt: 'Digital Comics Immagine'

                },{
                    id: 2,
                    title: 'Dc Merchandice',
                    src: './src/assets/img2/buy-comics-merchandise.png',
                    alt: 'Merchandise Immagine'
                },{
                    id: 3,
                    title: 'Subscription',
                    src: './src/assets/img2/buy-comics-subscriptions.png',
                    alt: 'Subscription Immagine'
                },{
                    id: 4,
                    title: 'Comic Shop Locator',
                    src: './src/assets/img2/buy-comics-shop-locator.png',
                    alt: 'Shop locator Immagine'
                },{
                    id: 5,
                    title: 'Dc Power Visa',
                    src: './src/assets/img2/buy-dc-power-visa.svg',
                    alt: 'DC Power VISA Immagine'
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
    <section>
        <article v-for="article in ArticleImgLinks" :key="article.id">
        <img :src="article.src" :alt="article.alt">
        <h2>
            {{ article.title }}
        </h2>
    </article>
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
    section{
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100%;
        width: 100%;
        article{
            display: flex;
            align-items: center;
            font-size: .5rem;
            text-transform: uppercase;
            color: $third_color;
        }
        img{
            height: 45px;
            padding: 1.5rem;
        }
    }
</style>
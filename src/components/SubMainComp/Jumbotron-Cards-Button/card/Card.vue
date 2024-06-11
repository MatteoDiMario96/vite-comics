<script>
export default {
    props:{
        singleCard: {
                type: Object,
                required: true,
            }
    },
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
    <div id="card">
            <img :src="singleCard.thumb" :alt="singleCard.series">
            <h3>
                {{ singleCard.series }}
            </h3>
        </div>
</template>

<style lang="scss" scoped>
    div#card{
            width: calc((100% / 6) - 1rem);
            margin-right: 1rem;
            margin-bottom: 1.5rem;
            img{
            width: 100%;
            /*Questa è quella giusta ma dovevo perforza far visualizzare bene per intero le card. Troppo belle. 
            height: 150px;*/
            height: 248px;
            object-fit: cover;
            object-position: top;
            margin-bottom: .4rem;
        }
        h3{
            text-align: start;
            font-size: .7rem;
            text-transform: uppercase;
            font-weight: 200;
        }
        }
</style>
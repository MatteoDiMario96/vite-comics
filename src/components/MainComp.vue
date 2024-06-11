<script>
    import MainSectionArticleComp from './SubMainComp/MainSectionArticleComp.vue';
    import JumbotronComp from './SubMainComp/Jumbotron-Cards-Button/JumbotronComp.vue';
    import CardsComp from './SubMainComp/Jumbotron-Cards-Button/CardsComp.vue';
    import ButtonComp from './SubMainComp/Jumbotron-Cards-Button/ButtonComp.vue';


export default {
    components:{
        MainSectionArticleComp,
        JumbotronComp,
        CardsComp,
        ButtonComp,
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
    <main>
        <div id="div-black">
            <section id="jumbotron">
                <JumbotronComp/>
            </section>
            <section id="black">
            <CardsComp/>
            <div id="button">
                <ButtonComp/>
            </div>
        </section>
        </div>
        <div id="div-blu">
            <section id="blu">
            <MainSectionArticleComp/>
        </section>
        </div>
    </main>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;
    section#jumbotron{
        background-image: url('../assets/img2/jumbotron.jpg');
        height: 285px;
        background-size: cover;
    }
    div#div-black{
        background-color: #1c1c1c;
    }
    section#black{
        background-color: #1c1c1c;
        padding: 1rem;
        // @include flex-center();
        color: $third_color;
        font-size: 1.6rem;
        display: flex;
        flex-direction: column;
        justify-content: center;
        max-width: $width_container;
        margin: 0 auto;
    }
    div#div-blu{
        background-color: $primary_color;
    }
    section#blu{
        height: 80px;
        padding: 1rem;
        display: flex;
        background-color: $primary_color;
        max-width: $width_container;
        margin: 0 auto;
    }
    div#button{
        margin: 0 auto;
    }
</style>
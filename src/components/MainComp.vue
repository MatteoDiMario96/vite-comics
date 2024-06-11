<script>
    import MainSectionArticleComp from './MainSectionArticleComp.vue';
export default {
    components:{
        MainSectionArticleComp,
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
        <section id="black">
            <p>
                -->Content goes here <--
            </p>
        </section>
        <section id="blu">
            <MainSectionArticleComp/>
        </section>
    </main>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    section#black{
        background-color: #1c1c1c;
        height: 70px;
        padding: 1rem;
        // @include flex-center();
        color: $third_color;
        font-size: 1.6rem;
        display: flex;
        flex-direction: column;
    }
    section#blu{
        height: 80px;
        padding: 1rem;
        display: flex;
        background-color: $primary_color;
    }
</style>
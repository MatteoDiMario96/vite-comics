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
    <main>
        <p>
            -->Content goes here <--
        </p>
    </main>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    main{
        background-color: #1c1c1c;
        height: 70px;
        padding: 1rem;
        @include flex-center();
        color: $third_color;
        font-size: 1.6rem;
    }
</style>
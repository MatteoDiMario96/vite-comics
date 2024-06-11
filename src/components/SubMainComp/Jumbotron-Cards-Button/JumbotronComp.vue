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
    <div class="container">
        <div>
        Current Series
    </div>
    </div>
</template>

<style lang="scss" scoped>
    @use '../../../styles/partials/variables' as *;
    div.container{
        max-width: $width_container;
        margin: 0 auto;
        div{
        text-transform: uppercase;
        background-color: $primary_color;
        display: inline-block;
        padding: .7rem .9rem .7rem .9rem;
        color: $third_color;
        position: relative;
        top: 270px;
        font-weight: 900;
    }
    }
    
</style>
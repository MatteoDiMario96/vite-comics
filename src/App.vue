<script>
  import HeaderComp from './components/HeaderComp.vue';
  import MainComp from './components/MainComp.vue';
  import FooterComp from './components/FooterComp.vue';

export default {
  components:{
    HeaderComp,
    MainComp,
    FooterComp,
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
    <div id="container">
      <HeaderComp/>

      <MainComp/>

      <FooterComp/>
    </div>
</template>

<style lang="scss">
  @use './styles/general.scss' as *;
  @use './styles/partials/variables' as *;
  @use './styles/partials/mixins' as *;
</style>

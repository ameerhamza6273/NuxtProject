<template>
    <div style="background-color: #FFF;">
        <AmbarHeroSection/>
        <AmbarCards/>
    </div>
  </template>
  <script>
  import AmbarHeroSection from '~/components/AmbarHeroSection.vue';
  import AmbarCards from '~/components/AmbarCards.vue';
  export default{
    name:"Ambar",
    components:{
        AmbarHeroSection,
        AmbarCards,
    },
    data(){
        return{
            pageTitle:'Ambar Immigration',
        }
    },
    mounted() {
        document.title = this.pageTitle;
    },
  }
  </script>
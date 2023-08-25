<template>
    <div style="background-color: #FFF;">
        <HerosectionFbprocess/>
        <prevallingFrame/>
        <FamilyFrame/>
    </div>
  </template>
  <script>
  import HerosectionFbprocess from '~/components/FbProcess/HerosectionFbprocess.vue';
  import prevallingFrame from '~/components/FbProcess/PrevallingFrame.vue';
  import FamilyFrame from '~/components/FbProcess/FamilyFrame.vue';
  export default{
    name:"Fbprocess",
    components:{
        HerosectionFbprocess,
        prevallingFrame,
        FamilyFrame
    },
    data(){
        return{
            pageTitle:'FB-3 Process',
        }
    },
    mounted() {
        document.title = this.pageTitle;
    },
  }
  </script>
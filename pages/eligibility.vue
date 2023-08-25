<template>
    <div style="background-color: #FFF;">
        <EligibilMain/>
        <EligibilContent/>
    </div>
  </template>
  <script>
  import EligibilMain from '~/components/EligibilMain.vue';
  import EligibilContent from '~/components/EligibilContent.vue';

  export default{
    name:"Eligibilty",
    components:{
      EligibilMain,
      EligibilContent,
    },
    data(){
        return{
            pageTitle:'Check Eligibility',
        }
    },
    mounted() {
        document.title = this.pageTitle;
    },
  }
  </script>
<template>
    <div>
        <JobMain/>
        <JobDetail/>
        <JobSlider/>
        <JonCards/>
    </div>
  </template>
  <script>
  import JobMain from '~/components/JobMain.vue';
  import JobDetail from '~/components/JobDetail.vue';
  import JobSlider from '~/components/JobSlider.vue';
  import JonCards from '~/components/JobCards.vue';
  export default{
    name:"jobs",
    components:{
      JobMain,
      JobSlider,
      JobDetail,
      JonCards,
    },
    data(){
        return{
            pageTitle:' jobs ',
        }
    },
    mounted() {
        document.title = this.pageTitle;
    },
  }
  </script>
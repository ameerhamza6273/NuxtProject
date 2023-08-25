<template>
    <div style="background-color: #FFF;">
        <EmployeMain/>
        <EmployeForm/>
        
    </div>
  </template>
  <script>
  import EmployeMain from '~/components/EmployeMain.vue';
  import EmployeForm from '~/components/EmployeeForm.vue';

  export default{
    name:"EmployerServices",
    components:{
      EmployeMain,
      EmployeForm,
    },
    data(){
        return{
            pageTitle:'Emloyer Services',
        }
    },
    mounted() {
        document.title = this.pageTitle;
    },
  }
  </script>
<template>
  <div style="background-color: #FFF;">
    <ContactMain />
    <ContactForm />
  </div>
</template>
<script>
import ContactMain from '~/components/ContactMain.vue';
import ContactForm from '~/components/ContactForm.vue';

export default {
  name: "ContactUs",
  components: {
    ContactMain,
    ContactForm,
  },
  data(){
        return{
            pageTitle:'Contact Us',
        }
    },
    mounted() {
        document.title = this.pageTitle;
    },
}
</script>
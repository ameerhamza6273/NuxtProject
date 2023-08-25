<template>
  <div style="background-color: #FFF;">
    <HeroSectinMain />
    <BrandsHome/>
    <ApplyFrameHome/>
    <GreenCardHome/>
    <IndividualHome />
    <TestimonialHome/>
    <ClientFrame />
    <ConfidenceHome/>
    <AskedQuestion />
    <ImageNavigater />
  </div>
</template>
<script>
import HeroSectinMain from '~/components/HeroSectinMain.vue';
import BrandsHome from '~/components/BrandsHome.vue';
import ApplyFrameHome from '~/components/ApplyFrameHome.vue';
import GreenCardHome from '~/components/GreenCardHome.vue';
import IndividualHome from '~/components/IndividualHome.vue';
import TestimonialHome from '~/components/TestimonialHome.vue';
import ClientFrame from '~/components/ClientFrame.vue';
import ConfidenceHome from '~/components/ConfidenceHome.vue';
import AskedQuestion from '~/components/AskedQuestion.vue';
import ImageNavigater from '~/components/ImageNavigater.vue';

export default {
  name: "Index",
  components: {
    HeroSectinMain,
    BrandsHome,
    ApplyFrameHome,
    GreenCardHome,
    IndividualHome,
    TestimonialHome,
    ClientFrame,
    ConfidenceHome,
    AskedQuestion,
    ImageNavigater,
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
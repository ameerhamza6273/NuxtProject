<template>
    <div>
        <v-container>
            <v-row class="individual-frame pa-3 mt-15">
                <!-- individual frame content is here-->
                <v-col cols="12" md="6" sm="12" class="individual-frame-inner">
                    <h1 class="individual-frame-heading font-weight-bold text-center text-md-left" color="#222222">
                        Individual Assistance Program (IAP)</h1>
                    <p class="individual-frame-text mt-6 font-weight-medium text-center text-md-left" color="#222222">
                        While the EB-3 Unskilled program is a long yet straightforward process, your personal circumstances
                        could make it unique.
                        We have started an Individual Assistance Program called IAP to help you before and after starting
                        your process.
                        If you think you are in a unique or complex situation, you may contact us to schedule a call.
                    </p>
                    <!-- individual frame button is here-->
                    <v-btn
                        class="individual-frame-btn d-block mx-auto ml-md-0 mt-sm-10 white--text mt-3 text-capitalize font-weight-medium rounded-lg"
                        height="65px" color="#041E42" width="210px">Schedule a Call</v-btn>
                </v-col>
                <!-- individual frame image is here-->
                <v-col cols="12" md="6" sm="12">
                    <img src="../assets/Image Placeholder (1).png" alt="user" class="individual-frame-img mt-9">
                </v-col>
            </v-row>
        </v-container>
    </div>
</template>

<script>
export default {
    name: "IndividualFrame",
    data() {
        return {
            // 
        }
    }
}
</script>

<style>
/* individual frame style is here */
.individual-frame {
    min-height: 500px;
}

.individual-frame-inner {
    align-self: center;
}

/* individual frame heading style is here */
.individual-frame-heading {
    font-family: 'Oswald';
    font-size: 34px;
    line-height: 45px;
    color: rgba(0, 0, 0, 0.87);
}

/* individual frame text style is here */
.individual-frame-text {
    font-family: 'Poppins';
    font-size: 16px;
    line-height: 25px;
    color: rgba(0, 0, 0, 0.87);
}

/* individual frame button style is here */

.individual-frame-btn {
    font-family: 'Poppins';
    font-size: 16px;
    line-height: 24px;
}
.individual-frame-img{
    width: 100%;
}
/* media queries start from here */
@media screen and (min-width:1900px) {
    .individual-frame {
        margin-left: 165px;
        margin-right: 145px;
    }
}

@media screen and (max-width:900px) {

    .individual-frame-img {
        min-height: 550px !important;
        
    }
}
</style>
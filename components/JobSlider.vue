<template>
    <div id="jombo-box" style="background-color: #FFF;">
        <v-container>
            <!-- job slider is here -->
            <carousel 
            :autoplay="false" 
            :loop="true" 
            :dots="false" 
            :center="true"
            :slide-by="1"
            :navclass="navClass"  
            :responsive="responsive">
                <v-row class="jombo-box rounded-xl">
                    <v-col cols="12" sm="1" class="jombo-box-img">
                        <img src="../assets/Commas.png" alt="" style="width: 40px">
                    </v-col>
                    <v-col cols="12" sm="11" class="pt-0 pr-0">
                        <h6 class="jombo-box-content font-weight-bold">Design comps, layouts, wireframes—will your clients
                            accept that you go
                            about things the facile way? Authorities in our business will tell in no uncertain
                            terms that Lorem Ipsum is that huge, huge no no to forswear forever. </h6>
                    </v-col> 
                </v-row>
                <v-row class="jombo-box rounded-xl">
                    <v-col cols="12" sm="1" class="jombo-box-img">
                        <img src="../assets/Commas.png" alt="" width="40px" style="width: 40px">
                    </v-col>
                    <v-col cols="12" sm="11" class="pt-0 pr-0">
                        <h6 class="jombo-box-content font-weight-bold">Design comps, layouts, wireframes—will your clients
                            accept that you go
                            about things the facile way? Authorities in our business will tell in no uncertain
                            terms that Lorem Ipsum is that huge, huge no no to forswear forever. </h6>
                    </v-col>
                </v-row>
            </carousel>
        </v-container>
    </div>
</template>

<script>
import carousel from 'vue-owl-carousel'
export default {
    name: "JobSlider",
    components: { carousel },
    data() {
        return {
            navClass: ["owl-prev", "owl-next"],
            // for responsive carousel --- 
            responsive: {
                0: {
                    items: 1,
                    nav: true
                },
                600: {
                    items: 1,
                    nav: true
                },
                900: {
                    items: 1,
                    nav: true
                }
            },
        }
    }
}
</script>

<style>
/* style is here */

.jombo-box {
    background: #F7F7F7;
    max-width: 980px;
    margin: 0 auto;
    width: 80%;
    padding: 45px 45px 35px 45px;
}

.jombo-box-content {
    font-family: 'Oswald';
    font-size: 32px;
    line-height: 40px;
    color: #222222;
}

#jombo-box .owl-theme .owl-nav [class*='owl-next'] {
    margin-left: 20px;
    background-color: transparent;
    position: absolute;
    right: 0;
}

#jombo-box .owl-theme .owl-nav [class*='owl-next']:hover {
    background-color: transparent;
}

#jombo-box .owl-theme .owl-nav [class*='owl-next'] img {
    width: 7px;
}

#jombo-box .owl-theme .owl-nav [class*='owl-next']::before {
    content: "Next Article";
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 500;
    font-size: 17px;
    color: #4997D3;
    top: -2px;
    position: relative;
}

#jombo-box .owl-theme .owl-nav [class*='owl-next']::after {
    content: url("./assets/Blue Right.png");
}

#jombo-box .owl-theme .owl-nav [class*='owl-prev'] {
    margin-right: 20px;
    background-color: transparent !important;
    position: absolute;
    left: 0px;
}

#jombo-box .owl-theme .owl-nav [class*='owl-prev'] img {
    width: 7px;
}

#jombo-box .owl-theme .owl-nav [class*='owl-prev']::after {
    content: "Previous Article";
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 500;
    font-size: 17px;
    color: #4997D3;
    top: -2px;
    position: relative;
}

#jombo-box .owl-theme .owl-nav [class*='owl-prev']::before {
    content: url("./assets/Blue Left.png");
}

/* media queries is here */
@media screen and (min-width:1900px) {
    #jombo-box {
        margin-left: 200px;
        margin-right: 200px;
    }

    .jombo-box {
        width: 90%;
    }

    #jombo-box .owl-theme .owl-nav [class*='owl-next'] {
        right: 125px;
    }

    #jombo-box .owl-theme .owl-nav [class*='owl-prev'] {
        left: 125px;
    }
}

@media screen and (max-width:1260px) {
    .jombo-box {
        width: 90%;
    }
}

@media screen and (max-width:800px) {
    .jombo-box-content {
        padding-left: 10px;
    }

    .jombo-box {
        width: 90%;
        padding: 30px 35px 30px 35px;
    }

    .jombo-box-img {
        padding-left: 0;
    }
}

@media screen and (max-width:450px) {
    .jombo-box-content {
        font-weight: 600;
        font-size: 27px;
        line-height: 37px;
    }

    #jombo-box .owl-theme .owl-nav [class*='owl-next']::before {
        font-size: 13px;
        right: -14px;
        top: -4px;
    }

    #jombo-box .owl-theme .owl-nav [class*='owl-prev']::after {
        font-size: 13px;
        left: -14px;
        top: -4px;
    }
}

</style>
<template>
    <div>
        <v-container>
            <!-- confidence content is here -->
            <div class="confidence mt-16">
                <p class="confidence-text text-center font-weight-medium">Apply with</p>
                <h1 class="confidence-heading font-weight-bold text-center mt-n2">Confidence</h1>
            </div>
            <!-- confidence cards is here -->
            <div class="confidence-inner mt-15" min-height="500px">
                <carousel :autoplay="false" :loop="true" :dots="false" :center="true" :slide-by="1" :navclass="navClass" :responsive="responsive">
                    <v-card 
                    v-for="(item, index) in confidenceCardsArray" id="confidence-card" :key="index" 
                    max-width="360" flat class="confidence-inner-cards rounded-xl" >
                        <img alt="user" :src="item.img" class="confidence-inner-cards-img d-block mx-auto">
                        <v-card-title class="confidence-inner-cards-heading mt-3 font-weight-bold">
                            {{ item.title }}
                        </v-card-title>
                        <v-card-text class="confidence-inner-cards-text text-center pb-0 font-weight-medium">
                            <p>{{ item.text }}</p>
                        </v-card-text>
                    </v-card>
                </carousel>
            </div>
            <div class="text-center">
                <v-btn class="confidence-btn d-block mx-auto white--text mt-3 text-capitalize font-weight-medium rounded-lg" height="65px" color="#041E42" width="190px">Apply Now</v-btn>
            </div>
        </v-container>
    </div>
</template>

<script>
import carousel from 'vue-owl-carousel'
export default {
    name: "ConfidenceHome",
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
                    items: 3,
                    nav: false
                }
            },
            confidenceCardsArray: [
                {
                    img: require("../assets/Happy Icon.png"), title: "Online application Process", text: `We have implemented a new online EB-3 unskilled application system that enables applicants to
                apply and track their application process online throughout their journey. Sign Up today.`},
                {
                    img: require("../assets/shieldtick.png"), title: "We care for your Privacy", text: `We strictly follow US privacy laws and don’t share your personal data with anyone not working on
                your application. We will not share your application details and updates with anyone without your prior consent.`},
                {
                    img: require("../assets/Happy Icon.png"), title: " Do what you Love", text: `The EB-3 Unskilled green card requires the applicant to work for the sponsor for one year.
                            Choose a job you like and fulfil your commitment.`},
            ]
        }
    }
}
</script>

<style>
/* confidence style is here */
.confidence .confidence-text {
    font-family: 'Poppins';
    font-size: 20px;
    line-height: 25px;
    color: #4172A0 !important;
}

.confidence .confidence-heading {
    font-family: 'Oswald';
    font-size: 40px;
    line-height: 50px;
    color: #222222 !important;
}

/*  confidence cards style is here*/

.confidence-inner-cards {
    margin-top: 100px;
    padding: 60px 5px 1px 5px;
    min-height: 380px;
    background-color: transparent !important;
}

.confidence-inner-cards-img {
    width: 75px !important;
}

.confidence-inner-cards-heading {
    justify-content: center;
    font-family: 'Poppins';
    font-size: 20px;
    line-height: 30px;
    color: #222222;
}

.confidence-inner-cards-text {
    font-family: 'Poppins';
    font-size: 16px;
    line-height: 24px;
    color: #111827 !important;
}

.confidence-btn {
    font-family: 'Poppins';
    font-size: 16px;
    line-height: 24px;
}

/* carousel style is here */
.confidence-inner .owl-item.active.center>div .confidence-inner-cards-heading {
    color: #FFFFFF !important;
}

.confidence-inner .owl-item.active.center>div .confidence-inner-cards-text {
    color: #FFFFFF !important;
}

.confidence-inner .owl-item.active.center>div .confidence-inner-cards-img {
    filter: brightness(7.25)
}

.confidence-inner .owl-item.active.center>div {
    background-color: #4172A0 !important;
    margin-top: 13px;
}

.confidence-inner .owl-theme .owl-nav [class*='owl-next'] {
    margin-left: 20px;
    background-color: transparent;
}
.confidence-inner .owl-theme .owl-nav [class*='owl-next']::after {
    content: url("./assets/Down_Arrow_3_ (1).png");
}

.confidence-inner .owl-theme .owl-nav [class*='owl-next']:hover {
    background-color: transparent;
}

.confidence-inner .owl-theme .owl-nav [class*='owl-prev'] {
    margin-right: 20px;
    background-color: transparent !important;
}
.confidence-inner .owl-theme .owl-nav [class*='owl-prev']::after {
    content: url("./assets/Down_Arrow_3_.png");
}

/* media queries is here */
@media screen and (min-width:1900px) {
    .confidence-inner {
        margin-left: 200px;

    }
}

@media screen and (max-width:1260px) {
    .confidence-inner-cards {
        padding: 50px 0px 1px 0px;
        min-height: 350px;
    }

    .confidence-inner-cards-heading {
        font-weight: 300;
        font-size: 18px;
        margin-top: 10px;
    }

    .confidence-inner-cards-text {
        font-weight: 100;
        font-size: 13px;
        margin-top: -10px;
    }

    .confidence-btn {
        margin-top: 10px;
    }
}

@media screen and (max-width:900px) {
    .confidence-inner-cards {
        margin: 0 auto;
        padding: 60px 5px 1px 5px;
        min-height: 380px;

    }

    .confidence-inner-cards-heading {
        font-weight: 500;
        font-size: 20px;
        margin-top: 15px;
    }

    .confidence-inner-cards-text {
        font-weight: 300;
        font-size: 16px;
        margin-top: 0px;
    }

    .confidence-btn {
        margin-top: 30px;
    }
}
</style>
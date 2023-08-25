<template>
    <div>
        <v-container>
            <v-row class="testimonial p-3 mt-15">
                <!-- testimonial title is here -->
                <v-col cols="12" lg="5" md="3" sm="12" class="testimonial-inner">
                    <h1 class="testimonial-inner-heading font-weight-bold">TESTIMONIALS</h1>
                    <p class="testimonial-inner-text mt-3 font-weight-medium">
                        What our Clients say!
                    </p>
                    <img src="../assets/Dots Ornament.png" alt="user" width="125px" class="testominail-image">
                </v-col>
                <!-- testimonial card is here -->
                <v-col cols="12" lg="7" md="9" sm="12">
                    <carousel 
                    :loop="true" 
                    :nav="true" 
                    :dots="false" 
                    :navclass="navClass" 
                    :responsive="responsive">
                        <v-card class="testimonial-card rounded-xl mx-2 pa-4 elevation-3" color="#041E42">
                            <v-card-text class="testimonial-card-text pb-0 white--text font-weight-medium">
                                <p>
                                    "Obtaining a green card through the EB3 process seemed like a daunting task, but thanks
                                    to
                                    the expertise and dedication of Ambar Immigration,
                                    it became a seamless journey. Their team guided me through every step, ensuring I had
                                    all
                                    the necessary documentation and keeping me informed throughout.
                                    I am grateful for their exceptional services and highly recommend Ambar Immigration to
                                    anyone seeking a green card.
                                </p>
                            </v-card-text>
                            <v-card-title class="white--text testimonial-profile">
                                <v-avatar size="58">
                                    <img alt="user" src="../assets/Image Placeholder (2).png">
                                </v-avatar>
                                <p class="ml-4 avatar-title">Ahmet</p>
                            </v-card-title>
                            <v-card-subtitle class="white--text avatar-subtitle mt-n10">Client from Turkey</v-card-subtitle>
                        </v-card> 
                        <v-card class="testimonial-card rounded-xl mx-2 pa-4 elevation-3" color="#041E42">
                            <v-card-text class="testimonial-card-text pb-0 white--text font-weight-medium">
                                <p>
                                    "Obtaining a green card through the EB3 process seemed like a daunting task, but thanks
                                    to
                                    the expertise and dedication of Ambar Immigration,
                                    it became a seamless journey. Their team guided me through every step, ensuring I had
                                    all
                                    the necessary documentation and keeping me informed throughout.
                                    I am grateful for their exceptional services and highly recommend Ambar Immigration to
                                    anyone seeking a green card.
                                </p>
                            </v-card-text>
                            <v-card-title class="white--text testimonial-profile">
                                <v-avatar size="58">
                                    <img alt="user" src="../assets/Image Placeholder (2).png">
                                </v-avatar>
                                <p class="ml-4 avatar-title">Ahmet</p>
                            </v-card-title>
                            <v-card-subtitle class="white--text avatar-subtitle mt-n10">Client from Turkey</v-card-subtitle>
                        </v-card>
                    </carousel>
                </v-col>
            </v-row>
        </v-container>
    </div>
</template>

<script>
import carousel from 'vue-owl-carousel'
export default {
    name: "TestimonialHome",
    components: { carousel },
    data() {
        return {
            navClass: ["owl-prev", "owl-next"],
            // for responsive carousel --- 
            responsive: {
                0: {
                    items: 1,
                },
                600: {
                    items: 1,
                },
                900: {
                    items: 1,
                }
            },
        }
    }
}
</script>

<style>
/* testimonial style is here */
.testimonial-inner-heading {
    font-family: 'Oswald';
    font-size: 38px;
    line-height: 40px;
    color: #222222;
}

.testimonial-inner-text {
    font-family: 'Poppins';
    font-size: 19px;
    line-height: 30px;
    color: #222222;
}

.testominail-image {
    display: -webkit-box;
    margin-left: auto;
    margin-top: 160px;
    margin-right: -52px;
}

/* testimonial card style is here */
.testimonial-card-text {
    font-family: 'Poppins';
    font-size: 16px;
    line-height: 25px;
    opacity: 0.75;
}

.avatar-title {
    font-family: 'Poppins';
    font-weight: 500;
    font-size: 17px;
    line-height: 30px;
}

.avatar-subtitle {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 100;
    font-size: 12px;
    line-height: 20px;
    margin-left: 72px;
}

/* owel carousel style is here */

.testimonial .owl-theme .owl-nav [class*='owl-next'] {
    position: absolute;
    left: -505px;
    top: 290px;
    background-color: transparent !important;
}
.testimonial .owl-theme .owl-nav [class*='owl-next']::before {
    content: url("./assets/Down_Arrow_bottom_.png");
}

.testimonial .owl-theme .owl-nav [class*='owl-prev'] {
    position: absolute;
    left: -505px;
    top: 229px;
    background-color: transparent !important;
}
.testimonial .owl-theme .owl-nav [class*='owl-prev']::before {
    content: url("./assets/Down_Arrow_top_ (1).png");
}

.testimonial .owl-theme .owl-nav [class*='owl-prev'] img {
    width: 25px;
}

.testimonial .owl-theme .owl-nav [class*='owl-next'] img {
    width: 25px;
}

/* media dueries star from here */

@media screen and (min-width:1900px) {
    .testimonial {
        margin-left: 165px;
        margin-right: 145px;
    }

    .testominail-image {
        margin-top: 118px;
    }

    .testimonial .owl-theme .owl-nav [class*='owl-next'] {
        left: -615px;
        top: 310px;
    }

    .testimonial .owl-theme .owl-nav [class*='owl-prev'] {
        left: -615px;
        top: 240px;
    }
}

@media screen and (max-width:1260px) {
    .testimonial-inner-heading {
        font-weight: 600;
        font-size: 32px;
        line-height: 30px;
    }

    .testimonial-inner-text {
        font-weight: 300;
        font-size: 16px;
        line-height: 25px;
    }

    .testominail-image {
        margin-top: 180px;
    }

    .testimonial .owl-theme .owl-nav [class*='owl-next'] {
        left: -230px;
        top: 310px;
    }

    .testimonial .owl-theme .owl-nav [class*='owl-prev'] {
        position: absolute;
        left: -230px;
        top: 240px;
    }
}

@media screen and (max-width:960px) {
    .testominail-image {
        display: none;
    }

    .testimonial-inner-heading {
        font-weight: 700;
        font-size: 38px;
        text-align: center;
        line-height: 40px;
    }

    .testimonial-inner-text {
        text-align: center;
        font-weight: 400;
        font-size: 19px;
        line-height: 30px;
    }
    .testimonial .owl-theme .owl-nav [class*='owl-next'] {
    position: inherit;
    transform: rotate(-90deg);
}

.testimonial .owl-theme .owl-nav [class*='owl-prev'] {
    position: inherit;
    transform: rotate(-90deg);
}
}</style>
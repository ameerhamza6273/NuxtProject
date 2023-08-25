<template>
    <div>
        <v-container>
            <v-row class="images-navigater pb-0 pa-4">
                <!-- Images Navigater header is here -->
                <h1 class="images-navigater-heading mt-15 font-weight-bold"> Navigating the EB3 Green Card Journey: Insights and Guidance</h1>
                <v-col cols="12" sm="9" class="pl-0">
                    <p class="images-navigater-text mt-1 font-weight-medium">Discover the step-by-step process of obtaining an EB3 green
                        card and unlock the opportunities of permanent residency in the United States.
                    </p>
                </v-col>
                <v-col cols="12" sm="3">
                    <span class="images-navigater-link d-none d-sm-flex text-right text-decoration-underline font-weight-medium justify-end">See More Articles</span>
                </v-col>
            </v-row>
            <v-row class="images-navigater-inner">
                <!-- Images Navigater header and first colum is here -->
                <v-col cols="12" lg="7" md="7" sm="12" class="images-navigater-inner-big pl-0">
                    <img src="../assets/Image Placeholder (4).png" alt="user" class="images-navigater-big-img">
                    <p class="images-navigater-inner-blue-text pt-4 font-weight-medium text-uppercase">Understanding the EB3 Green Card Program</p>
                    <h1 class="images-navigater-inner-heading font-weight-bold mt-n2">Demystifying the EB3 Green Card Process</h1>
                    <!-- profile detail is here -->
                    <v-card flat color="white">
                        <v-card-title class="ml-n3">
                            <v-avatar size="52">
                                <img alt="user" src="../assets/Image Placeholder (5).png">
                            </v-avatar>
                            <p class="ml-4 Image-title font-weight-bold">Angus Smith</p>
                        </v-card-title>
                        <v-card-subtitle class="Image-subtitle mt-n10 font-weight-medium">May 19, 2023</v-card-subtitle>
                    </v-card>
                </v-col>
                <!-- Images Navigater second colum is here -->
                <v-col cols="12" lg="5" md="5" sm="12">
                    <v-row class="images-navigater-small-images">
                        <v-col cols="12" md="12" sm="6">
                            <img src="../assets/Image Placeholder (6).png" alt="user" class="images-navigater-small-img">
                            <p class="images-navigater-inner-blue-text pt-4 font-weight-medium text-uppercase">Steps to Obtain an EB3 Green Card</p>
                            <h1 class="images-navigater-inner-heading font-weight-bold mt-n2">Step-by-Step Guide: How to Secure an EB3 Green Card
                            </h1>
                        </v-col>
                        <v-col cols="12" md="12" sm="6">
                            <img src="../assets/Image Placeholder (7).png" alt="user" class="images-navigater-small-img">
                            <p class="images-navigater-inner-blue-text pt-4 font-weight-medium text-uppercase">Strategies for a Successful EB3 Application</p>
                            <h1 class="images-navigater-inner-heading font-weight-bold mt-n2">Mastering the EB3 Application: Proven Strategies for
                                Success</h1>
                        </v-col>
                    </v-row>
                </v-col>
            </v-row>
            <span class="images-navigater-link d-flex d-sm-none mt-5 ml-4 text-decoration-underline font-weight-medium">See More Articles</span>
        </v-container>
    </div>
</template>

<script>

export default {
    name: "ImagesNavigater",
    data() {
        return {
            // 
        }
    }
}

</script>

<style>
/* .images navigater style is here*/
.images-navigater-heading {
    font-family: 'Oswald';
    font-size: 36px;
    line-height: 45px;
    color: #222222;
}

.images-navigater-text {
    font-family: 'Poppins';
    font-size: 16px;
    line-height: 27px;
    color: #222222;
    max-width: 785px;
}

.images-navigater-link {
    font-family: 'Poppins';
    font-size: 16px;
    line-height: 27px;
    color: #4172A0;
    cursor: pointer;
}

.images-navigater-inner {
    padding: 0 15px;
}

.images-navigater-big-img {
    width: 690px !important;
    height: 600px;
}

.images-navigater-small-img {
    max-width: 440px !important;
    max-height: 300px;
}

.images-navigater-inner-blue-text {
    font-family: 'Poppins';
    font-size: 14px;
    line-height: 21px;
    color: #4997D3;
}

.images-navigater-inner-heading {
    font-family: 'Oswald';
    font-size: 37px;
    line-height: 45px;
    color: #222222;
}

.images-navigater-inner .Image-title {
    font-family: 'Poppins';
    font-size: 18px;
    line-height: 30px;
    color: #222222;
}

.images-navigater-inner .Image-subtitle {
    margin-left: 55px;
    font-family: 'Poppins';
    font-size: 15px;
    line-height: 24px;
    color: #222222;
}

.images-navigater-small-images {
    margin-left: 10px;
}

/* media queries is here */
@media screen and (min-width:1900px) {
    .images-navigater{
        margin-left: 175px !important;
        margin-right: 130px;
    }
    .images-navigater-inner {
        margin-left: 175px !important;
        margin-right: 130px;
    }

    .images-navigater-big-img {
        width: 100% !important;
    }

    .images-navigater-small-img {
        width: 130%;

    }
}

@media screen and (max-width:1265px) {
    .images-navigater-big-img {
        width: 525px !important;
        height: 550px;

    }

    .images-navigater-small-img {
        width: 350px !important;
    }
}

@media screen and (max-width:965px) {
    .images-navigater-inner-big {
        margin-left: 10px;
        padding-right: 0;
    }

    .images-navigater-big-img {
        width: 95% !important;
    }
}

@media screen and (max-width:800px) {
    .images-navigater-small-images {
        margin-left: -15px;
    }
}

@media screen and (max-width:740px) {
    .images-navigater-small-img {
        width: 95% !important;
    }
}

@media screen and (max-width:600px) {
    .images-navigater-inner-big{
        margin-top: -35;
    }
    .images-navigater-big-img {
        width: 100%;
        height: 250px;
    }

    .images-navigater-small-img {
        width: 100% !important;
        height: 210px;
    }
}</style>
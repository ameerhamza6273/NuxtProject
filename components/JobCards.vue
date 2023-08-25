<template>
    <div id="job-card" style="background-color: #FFF !important;">
        <v-container>
            <div class="mt-15">
                <!-- job titles is here -->
                <p class="job-card-text font-weight-medium">P O P U L A R T O P I C S</p>
                <v-row>
                    <v-col cols="12" sm="9" class="pl-0 pt-0">
                        <h1 class="job-card-title ml-4 font-weight-bold">Ambar Blogs</h1>
                    </v-col>
                    <v-col cols="12" sm="3">
                        <span class="job-card-link d-none d-sm-flex mt-9 justify-end font-weight-medium text-uppercase">See More Articles</span>
                    </v-col>
                </v-row>
            </div>
            <!-- cards is here -->
            <v-row class="job-all-cards mt-7">
                <v-col cols="12" md="6" sm="12">
                    <v-card flat class="job-card-1">
                        <!-- <v-img src="../assets/Image Placeholder blue.png" alt="user" class="job-card-img align-end rounded-xl"> -->
                            <v-card-subtitle class="job-card-subtitle-top pl-0  white--text font-weight-medium">OPPORTUNITIES</v-card-subtitle>
                            <h1 class="job-card-heading white--text font-weight-bold">Empowering Unskilled Workers for a New Beginning</h1>
                            <v-card-title class="pl-0">
                                <v-avatar size="46">
                                    <img alt="user" src="../assets/Image Placeholder pro.png">
                                </v-avatar>
                                <p class="ml-3 job-card-profile-title white--text font-weight-medium">Angus Smith</p>
                            </v-card-title>
                            <v-card-subtitle class="job-card-subtitle-bottom mt-n10  white--text font-weight-medium">August 15, 2023</v-card-subtitle>
                        <!-- </v-img> -->
                    </v-card>
                </v-col>
                <v-col cols="12" md="6" sm="12">
                    <v-card flat class="job-card-2" style="background-color: #FFF;">
                        <!-- <v-img src="../assets/Image Placeholder agre.png" alt="user" class="job-card-img align-end rounded-xl"> -->
                            <v-card-subtitle class="job-card-subtitle-top pl-0 white--text font-weight-medium" >OPPORTUNITIES</v-card-subtitle>
                            <h1 class="job-card-heading white--text font-weight-bold">Empowering Unskilled Workers for a New Beginning</h1>
                            <v-card-title class="pl-0">
                                <v-avatar size="46">
                                    <img alt="user" src="../assets/Image Placeholder pro.png">
                                </v-avatar>
                                <p class="ml-3 job-card-profile-title white--text font-weight-medium">Angus Smith</p>
                            </v-card-title>
                            <v-card-subtitle class="job-card-subtitle-bottom mt-n10 white--text font-weight-medium">August 15, 2023</v-card-subtitle>
                        <!-- </v-img> -->
                    </v-card>
                </v-col>
            </v-row>
            <span class="job-card-link d-flex d-sm-none mt-5 ml-4">See More Articles</span>
        </v-container>
    </div>
</template>

<script>
export default {
    name: "JobCards",
    data() {
        return {
            //    
        }
    }
}
</script>

<style>
/* style is here */
.job-card-text {
    font-family: 'Poppins';
    font-size: 17px;
    line-height: 30px;
    color: #4997D3;
}

.job-card-title {
    font-family: 'Oswald';
    font-size: 80px;
    line-height: 100px;
    color: #222222;
}

.job-card-link {
    font-family: 'Poppins';
    font-size: 16px;
    line-height: 27px;
    color: #4172A0;
    margin-right: 10px;
    cursor: pointer;
}

/*  card style is here */
.job-card-1 {
    height: 500px;
    width: 100%;
    background-image: url('../assets/Image Placeholder blue.png');
    border-radius: 30px !important;
    background-position: center;
    background-size: cover;
    padding: 30px;
    padding-top: 48%;
}
.job-card-2 {
    height: 500px;
    background-image: url('../assets/Image Placeholder agre.png');
    width: 100%;
    border-radius: 30px !important;
    background-position: center;
    background-size: cover;
    padding: 30px;
    padding-top: 48%;
}

.job-card-img {
    max-height: 480px;
    padding: 25px 25px 10px 25px;
}
 
.job-card-heading {
    font-family: 'Oswald';
    font-size: 37px;
    line-height: 45px;
}

.job-card-profile-title {
    font-family: 'Poppins';
    font-size: 16px;
    line-height: 25px;
}

.job-card-subtitle-top {
    font-family: 'Poppins';
    font-size: 13px;
    line-height: 24px;
    opacity: 0.8;
    margin-bottom: -12px !important
}

.job-card-subtitle-bottom {
    font-family: 'Poppins';
    font-size: 12px;
    line-height: 24px;
    opacity: 0.8;
    margin-left: 42px;
}
/* media queries is here */
@media screen and (min-width:1900px) {
    #job-card-1,
    #job-card-2 {
    margin-left: 333px;
    margin-right: 333px;
}
}
@media screen and (max-width:960px) {
    .job-card-1,
    .job-card-2 {
    padding-top: 34%;
}
}
@media screen and (max-width:600px) {
    .job-card-link{
    float: left;
}
.job-card-title {
   text-align: center;
}
.job-card-text {
   text-align: center;
}
.job-card-1,
    .job-card-2 {
    padding-top: 50%;
}
}
@media screen and (max-width:465px) {
    .job-card-title {
    font-weight: 600;
    font-size: 60px;
    line-height: 80px;
}
.job-card-heading {
    font-weight: 600;
    font-size: 30px;
    line-height: 40px;
}
.job-card-img {
    padding: 10px 10px 5px 10px;
}
.job-card-1,
    .job-card-2 {
    padding-top: 69%;
}
}
</style>
<template>
    <div style="background-color: #FFF !important;">
    <v-footer class="mt-15" color="#041E42">
        <!-- <v-container> -->
        <v-row>
            <!-- footer first col of logo is here -->
            <v-col cols="12" xl="4" lg="4" md="4" sm="5" xs="10" class="footer-frame-one pl-0 pr-0">
                <div>
                    <img alt="Vuetify Logo" src="../assets/logo_footer.png" width="110" />
                    <p class="footer-frame-one-text font-weight-medium white--text mt-15">Discover the step-by-step process of obtaining
                        an EB3 green card and unlock the opportunities of permanent residency in the United States.</p>
                </div>
                <div class="footer-frame-company">
                    <h1 class="footer-frame-heading font-weight-bold white--text">Company</h1>
                    <div v-for="(item, index) in companeyNames" :key="index" class="mt-3">
                        <p class="footer-frame-links font-weight-medium white--text">{{ item }}</p>
                    </div>
                </div>

            </v-col>
            <!-- footer second col of company here -->
            <v-col cols="12" xl="5" lg="5" md="5" sm="7" xs="12" class="footer-frame-two pl-0 pr-0">
                <!-- footer third col of contact & social here -->
                <div class="footer-frame-contact">
                    <h1 class="footer-frame-heading font-weight-bold white--text">Contact</h1>
                    <div class="mt-3">
                        <p class="footer-frame-links font-weight-medium white--text">+1 (864) 770 4251</p>
                        <p class="footer-frame-links font-weight-medium white--text">info@ambarimmigration.com</p>
                        <p class="footer-frame-links font-weight-medium white--text">Office Address</p>
                        <p class="footer-frame-links mt-n4 font-weight-medium white--text">500 E McBee Ave., Greenville, SC 29601, United States</p>
                        <p class="footer-frame-links font-weight-medium white--text">Meeting Address</p>
                        <p class="footer-frame-links mt-n4 font-weight-medium white--text">1016 Old Boiling Springs Rd, Greer, SC 29650, United States</p>
                    </div>
                </div>
                <div class="footer-frame-social">
                    <h1 class="footer-frame-heading font-weight-bold white--text">Social</h1>
                    <div v-for="(item, i) in socialArray" :key="i" class="mt-3">
                        <p class="footer-frame-links font-weight-medium white--text">{{ item }}</p>
                    </div>
                </div>
            </v-col>
            <!-- footer last col of subscribe here -->
            <v-col cols="12" xl="3" lg="3" md="3" sm="8" xs="12" class="footer-frame-subscribe pl-0">
                <h1 class="footer-frame-heading font-weight-bold white--text">Subscribe</h1>
                <p class="footer-frame-links mt-3 font-weight-medium white--text">Subscribe to stay tuned for new web design and latest updates. Let's
                    do it! </p>
                <v-text-field class="submit-input-style" dense append-icon="Submit" label="Enter your email Address" placeholder="My Email ID" solo flat autofocus></v-text-field>
            </v-col>
        </v-row>
        <!-- footer bottom content is here -->
        <v-row class="footer-bottom pb-3 ">
            <p class="footer-bottom-text font-weight-medium white--text">© 2023 All Rights Reserved</p>
            <v-spacer></v-spacer>
            <v-row class="footer-bottom-img-div" align="center">
                <img alt="user" src="../assets/Vector (1).png" class="ml-8" >
                <img alt="user" src="../assets/Vector (2).png" class="ml-8" >
                <img alt="user" src="../assets/instagram.png" class="ml-8" >
                <img alt="user" src="../assets/linkedin.png" class="ml-8" >
                <img alt="user" src="../assets/whatsapp.png" class="ml-8">
            </v-row>
            <v-spacer></v-spacer>
            <div>
                <span class="footer-bottom-text font-weight-medium white--text">Privacy Policy</span>
                <span class="footer-bottom-text font-weight-medium white--text">Terms & Conditions</span>
            </div>
        </v-row>
        <div class="small-screen-text font-weight-medium white--text">
            <span class="small-screen-text-1">Privacy Policy</span>
            <span class="small-screen-text-2">Terms & Conditions</span>
            <p class="small-screen-text-3">© 2023 All Rights Reserved</p>
        </div>
        <!-- </v-container> -->
    </v-footer>
</div>
</template>

<script>

export default {
    name: "FooterFrame",

    data() {

        return {
            // array of object for company & social is here 
            companeyNames: ["Home", "Employer Service", "EB-3 Process", "Jobs", "Blogs", "About Us", "Contact Us"],
            socialArray: ["Facebook", "Twitter", "Instagram", "LinkedIn", "WhatsApp"]
        }
    }
}

</script>

<style>
/* all footer style is here */
.v-footer {
    padding: 80px 80px 15px 80px !important;
    position:inherit;
    bottom: 0;
}

.footer-frame-one {
    margin-left: -13px;
    display: flex;
}

.footer-frame-two{
    display: flex;
}

.footer-frame-one-text {
    font-family: 'Inter';
    font-size: 13px;
    line-height: 15px;
    opacity: 0.75;
    max-width: 200px;
}

/* footer heading style is here */
.footer-frame-heading {
    font-family: 'Inter';
    font-size: 14px;
    line-height: 24px;
}

/* footer all links and small text style is here */
.footer-frame-links {
    font-family: 'Inter';
    font-size: 12px;
    line-height: 16px;
    opacity: 0.95;
}

.footer-frame-company {
    margin-left: 80px;
}

.footer-frame-contact {
    margin-left: 80px;
}

.footer-frame-contact p {
    max-width: 190px;
}

.footer-frame-social {
    padding-left: 80px;
}

/* subscribe input style is here */
.footer-frame-subscribe .v-text-field.v-text-field--solo .v-label {
    font-family: 'Inter';
    font-style: normal;
    font-weight: 400;
    font-size: 13px;
    color: #B1B5BB;
}

.footer-frame-subscribe .submit-input-style .v-input__slot {
    margin: 20px 0px 0px 10px !important;
    border-radius: 0 !important;
    max-width: 350px !important;
    background-color: #FFFFFF !important;
    color: #4172A0 ;
}

.footer-frame-subscribe .submit-input-style {
    font-family: 'Inter';
    font-style: normal;
    font-weight: 400;
    font-size: 13px;
    color: #B1B5BB;
    margin-left: -10px;
}

.footer-frame-subscribe .submit-input-style .v-icon.v-icon {
    font-family: 'Inter';
    font-style: normal;
    font-weight: 400;
    font-size: 15px !important;
    line-height: 24px;
    color: #FFFFFF;
    background-color: #4172A0 !important;
    padding: 7px 23px 7px 23px;
}

/* footer last row style is here */

.footer-bottom{
    width: 100%;
}

.small-screen-text,
.footer-bottom-text{
    font-family: 'Inter';
    font-size: 13px;
    line-height: 24px;
    align-items: center;
    opacity: 0.85;
}
.footer-bottom-img-div {
    justify-content: space-around !important;
}

.small-screen-text{
    display: none;
}

/* media queries start from here */
@media screen and (min-width:1900px) {
    .footer-frame-company {
        margin-left: 150px;
    }
    .footer-frame-social {
        padding-left: 180px;
    }
}
@media screen and (max-width:1160px) {
    .footer-frame-company {
        margin-left: 30px;
    }

    .footer-frame-contact {
        margin-left: 30px;
    }

    .footer-frame-social {
        padding-left: 30px;
    }
}

@media screen and (max-width:960px) {
    .footer-frame-company {
        margin-left: 70px;
    }

    .footer-frame-contact {
        margin-left: 80px;
    }

    .footer-frame-social {
        padding-left: 50px;
    }
    .footer-bottom-img-div{
        width: 100%;
        justify-content: center !important;
        margin-top: 5px;
    }

    .footer-bottom-text{
        display: none;
    }
    .small-screen-text{
        display: block;
        width: 100%;
    }
    .small-screen-text-1{
        margin-top: 35px;
    }
    .small-screen-text-2{
        float: right;
        margin-top: 0px;
    }
    .small-screen-text-3{
        text-align: center;
        margin-top: 10px;
    }
    .footer-frame-subscribe{
        margin-left: -10px;
    }
}
@media screen and (max-width:800px) {
    .footer-bottom-img-div{
        margin-bottom: 15px;
    }
}
@media screen and (max-width:600px) {
    .v-footer {
        padding: 50px 50px 15px 50px !important;
    }

    .footer-frame-contact {
        margin-left: 0px;
    }

    .footer-frame-social {
        padding-left: 65px;
    }
}

@media screen and (max-width:450px) {
    .footer-frame-one {
        display: block;
    }
    .footer-frame-company {
        margin-left: 0px;
    }
    .footer-frame-two{
        display: block;
    }
    .footer-frame-contact {
        margin-left: -10px;
    }

    .footer-frame-social {
        padding-left: 0px;
        margin-left: -10px;
    }
    .footer-bottom-img-div{
        margin-left: -60px
    }
   
}

</style>
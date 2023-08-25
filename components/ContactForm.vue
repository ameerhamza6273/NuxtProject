<template>
    <div>
        <v-container>
            <div class="contact-form pa-3 pb-0">
                <div>
                    <!-- contact information is here -->
                    <h1 class="contact-form-title font-weight-bold text-center text-sm-left">CONTACT INFORMATION</h1>
                    <v-row class="mt-13">
                        <v-col cols="12" sm="6">
                            <p class="contact-form-blue-text mb-2 font-weight-medium text-center text-sm-left">PHONE</p>
                            <p class="contact-form-text font-weight-medium">+1 (864) 770 4251</p>
                        </v-col>
                        <v-col cols="12" sm="6">
                            <p class="contact-form-blue-text mb-2 font-weight-medium text-center text-sm-left">EMAIL</p>
                            <p class="contact-form-text d-none d-md-flex font-weight-medium" >info@ambarimmigration.com</p>
                            <p id="email-text" class="contact-form-text d-flex d-md-none font-weight-medium">info @ambarimmigration .com</p>
                        </v-col>
                    </v-row>
                    <v-row>
                        <v-col cols="12" sm="6">
                            <p class="contact-form-blue-text mb-2 font-weight-medium text-center text-sm-left">OFFICE ADDRESS</p>
                            <p class="contact-form-text pr-10 font-weight-medium">500 E McBee Ave., Greenville, SC 29601, United States</p>
                        </v-col>
                        <v-col cols="12" sm="6">
                            <p class="contact-form-blue-text mb-2 font-weight-medium text-center text-sm-left">MEETING ADDRESS</p>
                            <p class="contact-form-text font-weight-medium">1016 Old Boiling Springs Rd, Greer, SC 29650, United States</p>
                        </v-col>
                    </v-row>
                </div>
                <!-- contact form is here -->
                <h1 class="contact-form-title mt-10 font-weight-bold text-center text-sm-left">CONTACT US</h1>
                <v-form class="mt-14">
                    <v-row>
                        <v-col cols="12" sm="6" class="pb-0">
                            <label class="label-style font-weight-medium">FIRST NAME</label>
                            <v-text-field class="input-style  mt-2" placeholder="Amelia" outlined style="color: brown !important;"></v-text-field>
                        </v-col>
                        <v-col cols="12" sm="6" class="pb-0">
                            <label class="label-style font-weight-medium">LAST NAME</label>
                            <v-text-field class="input-style  mt-2" placeholder="Watson" outlined></v-text-field>
                        </v-col>
                    </v-row>
                    <v-row>
                        <v-col cols="12" sm="6">
                            <label class="label-style font-weight-medium">EMAIL ADDRESS</label>
                            <v-text-field class="input-style  mt-2" placeholder="example@mail.com" outlined></v-text-field>
                        </v-col>
                        <v-col cols="12" sm="6">
                            <label class="label-style font-weight-medium">PHONE NUMBER</label>
                            <v-text-field class="input-style  mt-2" placeholder="123 - 456 - 7890" outlined></v-text-field>
                        </v-col>
                    </v-row>
                    <label class="label-style font-weight-medium">Message</label>
                    <v-textarea class="input-style mt-2" auto-grow placeholder="Message here" outlined rows="5"></v-textarea>
                    <v-btn class="contact-form-btn d-block mx-auto rounded-lg mt-4 text-capitalize white--text font-weight-medium" width="150px" height="60px" color="#041E42">Submit</v-btn>
                </v-form>
            </div>
        </v-container>
    </div>
</template>

<script>
export default {
    name: "ContactForm",
    data() {
        return {
            // 
        }
    }
}

</script>
<style>
/* style is here */

.contact-form-title {
    font-family: 'Oswald';
    font-size: 37px;
    line-height: 45px;
    color: #222222;
}

.contact-form-blue-text {
    font-family: 'Poppins';
    font-size: 23px;
    line-height: 35px;
    letter-spacing: 0.25em;
    color: #4172A0;
}

.contact-form-text {
    font-family: 'Poppins';
    font-size: 23px;
    line-height: 30px;
    color: #222222;
    max-width: 470px;
}

.contact-form .label-style {
    font-family: 'Poppins';
    font-size: 18px;
    line-height: 28px;
    color: #222222;
}

.contact-form .input-style {
    border-radius: 15px !important;
}

.contact-form .input-style .v-input__control .v-input__slot {
    background-color:#F7F7F7;
}

.contact-form .v-text-field>.v-input__control>.v-input__slot fieldset {
    border-color: #F7F7F7 !important;
}

.contact-form .v-input--is-focused .v-input__slot {
    border: 2px solid #4172A0 !important;
}
.contact-form .v-input--is-focused .v-input__control .v-text-field__slot {
    padding: 10px;
}

.contact-form .input-style .v-input__control .v-text-field__slot {
    padding: 15px !important;
}

/* .contact-form .input-style .v-input__control .v-text-field__slot::placeholder {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    line-height: 30px;
    color: #6B7280 !important;
    opacity: 0.75;
} */

.contact-form-btn {
    font-family: 'Poppins';
    font-size: 16px;
    line-height: 24px;
}

/* media queries is here */
@media screen and (min-width:1900px) {

    .contact-form {
        margin-left: 190px;
        margin-right: 175px;
    }
}
@media screen and (max-width:600px) {

    /* .contact-form-title {
       text-align: center;
    }
    .contact-form-blue-text{
        text-align: center;
    } */
    #email-text{
        justify-content: center;
    }
    .contact-form-text{
        text-align: center;
        max-width: 100%;
    }
}
</style>
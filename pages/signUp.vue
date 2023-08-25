
<template>
    <div>
        <v-responsive>
            <v-row class="signup">
                <!-- image column is here -->
                <v-col cols="12" md="4" sm="12" class="signup-frame1">
                    <div class="signup-content">
                        <img src="../assets/logo_footer.png" alt="user" class="signup-img">
                        <h1 class="signup-heading font-weight-bold text-center mt-3">Access Your Green Card
                            Journey</h1>
                        <p class="signup-text text-center font-weight-medium mt-2">Login or Sign Up to access
                            your personalized green card journey with Ambar
                            Immigration. By logging in
                            or signing up, you can take advantage of our tailored services, track your application progress,
                            and
                            receive important updates and notifications. Join us today and let us guide you towards
                            achieving
                            your green card and realizing your American Dream.</p>
                    </div>
                </v-col>
                <!-- form column is here -->
                <v-col cols="12" md="8" sm="12" style="background-color: #FFF;">
                    <div class="signup-inner" style="padding: 35px 0;">
                        <!-- form title is here -->
                        <h1 class="signup-inner-title font-weight-bold">Create an Account</h1>
                        <p class="signup-inner-text font-weight-medium">Don’t have an account? <span
                                class="signup-inner-bluetext text-center font-weight-bold">Log in
                                here</span></p>
                        <!-- google & facebook buttons is here -->
                        <div class="signup-inner-btns">
                            <v-btn class="signup-inner-btn font-weight-medium " outlined><img src="../assets/Logo (1).png" alt="user" width="17px"> Log in with Google</v-btn>
                            <v-btn id="btn2" class="signup-inner-btn  font-weight-medium " outlined ><img src="../assets/Logo (2).png" alt="user" width="17px">Log in with Facebook</v-btn>
                        </div>
                        <v-divider class="mt-5 mb-3"></v-divider>
                        <p class="line my-2">OR</p>
                        <!-- form is here -->
                        <v-form class="signup-form">
                            <v-row>
                                <v-col cols="12" sm="6">
                                    <label class="label-style font-weight-medium">First Name</label>
                                    <v-text-field class="input-style hide-details" placeholder="Emma" outlined></v-text-field>
                                </v-col>
                                <v-col cols="12" sm="6">
                                    <label class="label-style font-weight-medium">Last Name</label>
                                    <v-text-field class="input-style hide-details" placeholder="Watson" outlined></v-text-field>
                                </v-col>
                            </v-row>
                            <v-row style="margin-top: -34px;">
                                <v-col cols="12" sm="6">
                                    <label class="label-style font-weight-medium">Email</label>
                                    <v-text-field class="input-style hide-details" placeholder="someone@ambar.com" outlined></v-text-field>
                                </v-col>
                                <v-col cols="12" sm="6">
                                    <label class="label-style font-weight-medium">Country of Birth</label>
                                    <v-select class="input-style hide-details" append-icon="mdi-chevron-down" placeholder="select country of birth" outlined></v-select>
                                </v-col>
                            </v-row>
                            <div style="margin-top: -22px;">
                                <label class="label-style font-weight-medium">Password</label>
                                <v-text-field class="input-style" placeholder="***********" outlined hint="Use 8 or more characters with a mix of letters, numbers & symbols." persistent-hint append-icon="mdi-eye-off"></v-text-field>
                            </div>
                            <v-row>
                                <v-checkbox color="indigo" hide-details size="4" style="margin-left: 10px;"></v-checkbox>
                                <p class="label-style" style="font-size: 14px; line-height: 24px; margin-top: 20px; margin-left: 8px;">I agree to the <span style="text-decoration: underline;color: #4172A0;">Terms & Conditions</span></p>
                            </v-row>
                            <v-btn class="signup-btn font-weight-medium" @click="signUp()">Sign up</v-btn>
                        </v-form>
                    </div>
                </v-col>
            </v-row>
        </v-responsive>
    </div>
  </template>
  
  <script>
  
  export default {
    name: "Signup",
    data() {
        return {
            // 
        }
    },
    methods: {
        signUp() {
          this.$router.push("/login");
        }
    }
  }
  
  </script>
  
  <style>
  /* style is here */
  
  .signup-frame1 {
    /* background-image: url("@/assets/Rectangle\ 465.png") !important; */
    background-image: url("../assets/Rectangle 465.png")  !important;
    min-height: 104vh;
    background-position: center;
    background-size: cover;
    position: relative;
  }
  
  .signup-content {
    position: absolute;
    top: 40%;
    left: 30%;
    transform: translate(-20%, -20%);
  }
  
  .signup-img {
    max-width: 135px;
    margin: 0 auto !important;
    display: block;
  }
  
  .signup-heading {
    font-family: 'Oswald';
    font-size: 27px;
    line-height: 40px;
    color: #FFF;
  }
  
  .signup-text {
    font-family: 'Poppins';
    font-size: 11px;
    line-height: 20px;
    opacity: 0.9;
    color: #FFF;
  }
  
  /* signup inner style is here */
  
  .signup-inner-title {
    font-family: 'Oswald';
    font-size: 30px;
    line-height: 40px;
    color: #041E42;
    text-align: center;
  }
  
  .signup-inner-text {
    font-family: 'Poppins';
    font-size: 14px;
    line-height: 30px;
    color: #9CA3AF;
    text-align: center;
    margin-top: 4px;
    margin-bottom: 7px;
  }
  
  .signup-inner-bluetext {
    font-family: 'Poppins';
    font-size: 16px;
    line-height: 30px;
    color: #4172A0;
  }
  .signup-inner-btns{
    text-align: center;
  }
  
  .signup-inner-btn {
    font-family: 'Inter';
    font-size: 13px !important;
    line-height: 20px;
    border: 1px solid #E0E0E9;
    text-transform: inherit;
    margin: 0 15px;
    padding-right: 50px !important;
    text-align: center;
    border-radius: 8px;
    color: black !important;
  }
  .signup-inner-btn img{
   margin-right: 8px;
  }
  .signup-inner .v-divider {
    display: none;
  }
  
  .signup-inner .line {
    font-family: 'Poppins';
    font-size: 1rem;
    line-height: 30px;
    color: #9CA3AF;
    text-align: center;
  }
  
  .signup-inner .line::before,
  .signup-inner .line::after {
    display: inline-block;
    content: "";
    border-top: 1px solid #9ca3afb4 !important;
    transform: rotate(-180deg);
    width: 14rem;
    margin: -10px 1rem;
    transform: translateY(-1rem);
    top: 20px;
  }
  
  /* form style is here */
  .signup-inner .label-style {
    font-family: 'Poppins' !important;
    font-size: 16px;
    color: #222222;
  }
  
  .signup-inner .signup-form {
    display: table;
    margin-left: auto;
    margin-right: auto;
    min-width: 510px !important;
  }
  
  .signup-inner .input-style .v-input__control .v-input__slot {
    background-color: #F7F7F7;
    margin-bottom: 0;
    border-radius: 8px;
  }
  
  .signup-inner .v-text-field>.v-input__control>.v-input__slot fieldset {
    border-color: #F7F7F7 !important;
  }
  
  .signup-inner .v-input--is-focused .v-input__slot {
    border: 2px solid #4172A0 !important;
  }
  
  .signup-inner .input-style .v-input__control .v-text-field__slot {
    padding: 10px !important;
  }
  
  .v-select.v-text-field:not(.v-text-field--single-line) input {
    padding-left: 10px;
  }
  
  .signup-inner .theme--light.v-input input{
    font-family: 'Poppins' !important;
    font-style: normal;
    font-weight: 400;
    font-size: 14px;
    line-height: 30px;
    color: #6B7280;
    opacity: 0.75;
  }
  
  .signup-inner .input-style::placeholder {
    font-family: 'Poppins' !important;
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    line-height: 30px;
    color: #6B7280;
    opacity: 0.75;
  }
  
  .signup-inner .input-style .v-messages__message {
    font-family: 'Poppins' !important;
    margin-top: 5px !important;
    margin-left: -10px !important;
  }
  
  .signup-inner .input-style .mdi-eye-off::before {
    margin-right: 25px !important;
    font-size: 0.8em;
  }
  
  .signup-inner .signup-btn {
    font-family: 'Poppins';
    font-size: 16px;
    line-height: 24px;
    text-transform: inherit;
    height: 50px !important;
    background-color: #041E42 !important;
    margin: 0 auto;
    display: block;
    margin-top: 10px;
    color: #FFF;
    padding: 10px 60px;
    width: 160px;
    margin-top: 27px;
    border-radius: 8px;
  }
  
  /* media quires is here */
  @media screen and (max-width:960px) {
    .signup-frame1 {
        display: none;
    }
  
    .signup {
        padding: 10px;
    }
  }
  
  @media screen and (max-width:560px) {
    .signup-inner .signup-form {
        min-width: 210px !important;
        max-width: 450px;
    }
  
    .signup-inner .line {
        display: none;
    }
  
    .signup-inner .v-divider {
        display: block;
        margin: 0 7%;
    }
  
    #btn2 {
        margin-top: 15px;
    }
  
    .signup-inner-btns {
        margin-top: 25px;
    }
  }
  
  @media screen and (max-width:500px) {
    .signup-inner .v-divider {
        display: block;
        margin: 0 0%;
    }
  }</style>
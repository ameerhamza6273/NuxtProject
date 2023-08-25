<template>
    <div id="check-content" class="p-3">
        <v-container>
            <v-row class="check-content">
                <!-- small column is here -->
                <v-col cols="12" lg="4" md="4" sm="6">
                    <v-text-field label="Search" color="blach" append-icon="mdi-magnify"></v-text-field>
                    <!-- all buttens is here -->
                    <h4 class="check-content-title text-center text-sm-left mt-10 font-weight-bold">CATEGORIES</h4>
                    <v-row class="mt-5 pl-2 check-content-all-battuns">
                        <v-btn class="check-content-btn font-weight-medium text-capitalize" depressed color="primary">All</v-btn>
                        <v-btn v-for="(item, index) in buttensArray" :key="index" style="background-color: rgba(128, 128, 128, 0.082) !important;" class="check-content-btn font-weight-medium text-capitalize" depressed >{{ item.text }}</v-btn>
                    </v-row>
                    <v-divider class="mt-10" max-width="300px"></v-divider>
                    <!-- papular cards is here -->
                    <h4 class="check-content-title mt-8 font-weight-bold text-center text-sm-left">POPULAR</h4>
                    <div class="mt-4">
                        <v-card v-for="(item, index) in papularCardArray" :key="index" class="papular-card" flat color="white">
                            <img :src="item.img" alt="user" class="papular-card-img" width="100%" >
                            <v-card-text class="ml-n3 pb-0 pt-2">
                                <p class="papular-card-bluetext mb-1 font-weight-medium text-center text-sm-left">{{ item.bluText }}</p>
                                <h4 class="papular-card-title font-weight-bold text-center text-sm-left">{{ item.title }}</h4>
                                <p class="papular-card-subtitle text-center text-sm-left" style="color: rgba(0, 0, 0, 0.6);;">{{ item.subtitle }}</p>
                            </v-card-text>
                        </v-card>
                    </div>
                </v-col>
                <!-- big side column is here -->
                <v-col cols="12" lg="8" md="8" sm="6">
                    <h4 class="check-content-title mt-5 font-weight-bold text-center text-sm-left">CATEGORIES</h4>
                    <v-card flat color="white">
                        <img src="../assets/Image Placeholder Recent (1).png" alt="" width="100%" class="mt-12">
                        <v-card-text>
                            <p class="recent-card-bluetext font-weight-medium mb-1 text-center text-sm-left">EB-3 Visa</p>
                            <h4 class="recent-card-title font-weight-bold text-center text-sm-left">Empowering Unskilled
                                Workers for a New Beginning</h4>
                        </v-card-text>
                        <v-card-title class="recent-awatar pt-0">
                            <v-avatar size="50">
                                <img alt="user" src="../assets/Recent Profile.png">
                            </v-avatar>
                            <p class="ml-4 recent-awatar-title font-weight-bold">Angus Smith</p>
                        </v-card-title>
                        <v-card-subtitle class="recent-awatar-subtitle mt-n10 font-weight-medium">August 15,
                            2023</v-card-subtitle>
                    </v-card>
                    <!-- big side column small cards is here -->
                    <v-row class="mt-5">
                        <v-col cols="12" lg="6" md="6" sm="12">
                            <img src="../assets/Image Placeholder Recent (2).png" alt="user" width="100%">
                            <p class="recent-card-bluetext font-weight-medium mb-1 text-center text-sm-left">EB-3 Visa</p>
                            <h4 class="recent-card-title font-weight-bold text-center text-sm-left">How the EB3 Visa Empowers Unskilled Workers</h4>
                        </v-col>
                        <v-col cols="12" lg="6" md="6" sm="12">
                            <img src="../assets/Image Placeholder Recent  (3).png" alt="user" width="100%">
                            <p class="recent-card-bluetext font-weight-medium mb-1 text-center text-sm-left">SUCCESS</p>
                            <h4 class="recent-card-title font-weight-bold text-center text-sm-left">Inspiring Tales of Unskilled Workers Thriving in
                                the USA</h4>
                        </v-col>
                    </v-row>
                    <v-row>
                        <v-col cols="12" lg="6" md="6" sm="12">
                            <img src="../assets/Image Placeholder Recent  (4).png" alt="user" width="100%">
                            <p class="recent-card-bluetext font-weight-medium mb-1 text-center text-sm-left">OPPORTUNITIES</p>
                            <h4 class="recent-card-title font-weight-bold text-center text-sm-left">How the EB3 Visa Opens Doors for Unskilled
                                Workers</h4>
                        </v-col>
                        <v-col cols="12" lg="6" md="6" sm="12">
                            <img src="../assets/Image Placeholder Recent  (5).png" alt="user" width="100%">
                            <p class="recent-card-bluetext font-weight-medium mb-1 text-center text-sm-left">EB-3 Visa</p>
                            <h4 class="recent-card-title font-weight-bold text-center text-sm-left">Empowering Unskilled Workers for a New Beginning
                            </h4>
                        </v-col>
                    </v-row>
                </v-col>
            </v-row>
        </v-container>
    </div>
</template>

<script>

export default {
    name: "CheckContent",
    data() {
        return {

            buttensArray: [
                { text: "Fee Structure" }, { text: "Legal" }, { text: "Green Card" }, { text: "Workforce" },
                { text: "Jobs" }, { text: "Visa Process" }, { text: "Legal" }, { text: "Labor Market" },
            ],
            papularCardArray: [
                { img: require('@/assets/Image Placeholder  Popular (1).png'), bluText: "EB-3 Visa", title: " A Comprehensive Guide for Unskilled Workers", subtitle: "April 3, 2023" },
                { img: require('@/assets/Image Placeholder Popular  (2).png'), bluText: "OPPORTUNITIES", title: "How the EB3 Visa Opens Doors for Unskilled Workers", subtitle: "March 12, 2023" },
                { img: require('@/assets/Image Placeholder Popular  (3).png'), bluText: "EB-3 VISA", title: "Your Pathway to a Rewarding Career in the United States", subtitle: "February 17, 2023" },
                { img: require('@/assets/Image Placeholder Popular  (4).png'), bluText: "EB-3 VISA", title: "A Bridge to Success for Unskilled Workers", subtitle: "January 8, 2023" },
           
            ]
        }
    }
}

</script>

<style>
/* input style is here */
.check-content .v-text-field>.v-input__control>.v-input__slot {
    padding: 5px;
    max-width: 325px;
}

/* title style is here */
.check-content .check-content-title {
    font-family: 'Oswald';
    font-size: 37px;
    line-height: 45px;
    color: #222222;
}

/* buttons style is here */
.check-content .check-content-btn {
    margin: 4px;
    font-family: 'Poppins';
    font-size: 14px;
    line-height: 25px;
    color: #222222;
}

.check-content .v-divider {
    max-width: 325px;
}

/* papular cards style is here */
.papular-card {
    max-width: 87%;
}

.check-content .papular-card-bluetext {
    font-family: 'Poppins';
    font-size: 16px;
    line-height: 24px;
    color: #4172A0;
}

.check-content .papular-card-title {
    font-family: 'Poppins';
    font-size: 20px;
    line-height: 30px;
    color: #222222;
}

/* recent card style is here */
.check-content .recent-awatar-title {
    font-family: 'Poppins';
    font-size: 19px;
    line-height: 35px;
    color: #222222;
}

.check-content .recent-awatar-subtitle {
    font-family: 'Poppins';
    font-size: 14px;
    line-height: 24px;
    color: #222222;
    margin-left: 65px;
}

.check-content .recent-card-bluetext {
    font-family: 'Poppins';
    font-size: 16px;
    line-height: 24px;
    color: #4172A0;
}

.check-content .recent-card-title {
    font-family: 'Poppins';
    font-size: 26px;
    line-height: 35px;
    color: #222222;
}

/* media quieres is here */
@media screen and (min-width:1900px) {
    .check-content {
        margin-left: 190px;
        margin-right: 175px;
    }
}

@media screen and (max-width:600px) {
    .check-content .v-text-field>.v-input__control>.v-input__slot {
        margin: 0 auto !important;
    }

    .check-content .v-divider {
        max-width: 100% !important;
    }

    .check-content-all-battuns {
        justify-content: center;
    }

    .papular-card {
        max-width: 100%;
    }

}
</style>
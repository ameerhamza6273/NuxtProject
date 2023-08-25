<template>
    <div id="question" class="mt-15">
        <v-container>
            <!-- asked question content is here -->
            <div class="asked-question pt-15">
                <div class="asked-question-heading font-weight-bold white--text text-center">Frequently Asked Questions (FAQs)</div>
                <p class="asked-question-text mt-3 white--text text-center font-weight-medium">What our clients usually asked about our services and process.</p>
            </div>
            <!-- exponansion panel is here -->
            <v-row class="asked-question-expansion justify-center d-block mx-auto mt-6">
                <v-expansion-panels v-model="panel" accordion flat >
                    <v-expansion-panel v-for="(item, index) in expansionArray" :key="index" class="asked-question-expansion-style mt-7 rounded-xl elevation-3" :active-class="activeClass"  style="background-color: #FFF !important;">
                        <v-expansion-panel-header class="asked-question-expansion-title font-weight-medium" @click="marker = !marker">
                            {{ item.title }}
                        </v-expansion-panel-header>
                        <v-expansion-panel-content class="asked-question-expansion-text font-weight-medium">
                            {{ item.text }}
                        </v-expansion-panel-content>
                    </v-expansion-panel>
                </v-expansion-panels>
            </v-row>
        </v-container>
    </div>
</template>

<script>

export default {
    name: "AskedQuestion",
    data() {
        return {
            marker: true,
            panel: 0,
            // array of object for expansion panels is here
            expansionArray: [
                {
                    title: "What is the EB3 program?", text: `The EB-3 Unskilled is a job-based immigration offered since 1990. 
                This program offers a US green card and the opportunity to come, work and live permanently in the United States.`},
                {
                    title: "What services does Ambar Immigration officer?", text: `The EB-3 Unskilled is a job-based immigration offered since 1990. 
                This program offers a US green card and the opportunity to come, work and live permanently in the United States.`},
                {
                    title: "Does Ambar Immigration help find the sponsor?", text: `The EB-3 Unskilled is a job-based immigration offered since 1990. 
                This program offers a US green card and the opportunity to come, work and live permanently in the United States.`},
                {
                    title: "How long does the EB-3 Unskilled process take?", text: `The EB-3 Unskilled is a job-based immigration offered since 1990. 
                This program offers a US green card and the opportunity to come, work and live permanently in the United States.`},
                {
                    title: "Do I have to do an interview with the employer?", text: `The EB-3 Unskilled is a job-based immigration offered since 1990. 
                This program offers a US green card and the opportunity to come, work and live permanently in the United States.`},
            ]
        }
    },
    computed: {
    activeClass() {
      return this.edited ? 'active-panel-edited' : 'active-panel-normal';
    }
    }
}

</script>

<style>

/* asked question style is here */
#question {
    background-color: #041E42 !important;
    min-height: 770px;
    padding-bottom: 20px;
}

.asked-question-heading {
    font-family: 'Oswald';
    font-size: 40px;
    line-height: 50px;
}

.asked-question-text {
    font-family: 'Poppins';
    font-size: 20px;
    line-height: 30px;
    opacity: 0.75;
}

/* expansion panel style is here */

.asked-question-expansion {
    max-width: 800px;
}

.asked-question-expansion-title {
    font-family: 'Inter';
    font-size: 19px;
    line-height: 28px;
    color: #222222;
}

.asked-question-expansion-text {
    font-family: 'Poppins';
    font-size: 15px;
    line-height: 24px;
    color: #222222;
}

/* expansion panel icon style is here */
.v-application--is-ltr .v-expansion-panel-header__icon {
    border-radius: 50%;
    padding: 4px;
    border: 1px solid #4172A0;
}

.v-application--is-ltr .v-expansion-panel-header__icon .mdi-chevron-down{
    color: #4172A0 !important;
}

#question .active-panel-normal .v-expansion-panel-header__icon{
    background-color: #4172A0 !important;
}

#question .active-panel-normal .v-expansion-panel-header__icon .mdi-chevron-down{
    color: #FFFFFF !important;
}

</style>
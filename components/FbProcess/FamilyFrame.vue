<template>
    <div>
        <v-container>
            <!-- family frame title & text is here -->
            <div class="family-frame p-4 mt-10">
                <h1 class="family-frame-heading font-weight-bold text-center">Family of EB-3 Visa Holders</h1>
                <p class="family-frame-text mt-3 font-weight-medium text-center">If your I-140 petition is approved, your
                    spouse and unmarried children under the age of 21 may be eligible to apply for admission to the United
                    States
                    in EW4 (spouse of an “other worker”), and EW5 (child of an “other worker”).</p>
                <v-btn class="family-frame-btn mt-10 d-block text-capitalize mx-auto rounded-lg font-weight-medium white--text" width="190px" height="65px" color="#041E42">Apply Now</v-btn>
            </div>
        </v-container>
    </div>
</template>

<script>

export default {
    name: "FamilyFrame",
    data() {
        return {
            //    
        }
    }
}
</script>

<style>
/* style is here */

.family-frame-heading {
    font-family: 'Oswald';
    font-style: normal;
    font-size: 40px;
    line-height: 50px;
    color: #222222;
}

.family-frame-text {
    font-family: 'Poppins';
    font-size: 17px;
    line-height: 25px;
    color: #111827;
}

.family-frame-btn {
    font-family: 'Poppins';
    font-size: 16px;
    line-height: 24px;
}

/* media quries is here */
@media screen and (min-width:1900px) {
    .family-frame {
        margin-left: 165px;
        margin-right: 145px;
    }
}</style>
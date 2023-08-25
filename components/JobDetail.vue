<template>
    <div id="job-detail" class="p-4" style="background-color: #FFF !important;">
        <v-container>
            <!-- job title and text without images -->
            <div class="job-detail">
                <h1 class="job-detail-title text-center font-weight-bold">Empowering Foreign Workers for a New Beginning</h1>
                <p class="job-detail-text mt-5 font-weight-medium">Design comps, layouts, wireframes—will your clients accept that you go about
                    things
                    the facile way? Authorities in our business will tell in no uncertain terms that Lorem Ipsum is that
                    huge, huge no no to forswear forever.</p>
                <p class="job-detail-text mt-5 font-weight-medium">The toppings you may chose for that TV dinner pizza slice when you forgot to shop
                    for foods, the paint you may slap on your
                    face to impress the new boss is your business. But what about your daily bread? Not so fast, I'd say,
                    there are some redeeming factors in
                    favor of greeking text, as its use is merely the symptom of a worse problem to take into consideration.
                </p>
            </div>
            <!-- job text and images -->
            <div class="job-terms">
                <h3 class="job-terms-title mt-5 mb-4 text-center font-weight-medium">uncertain terms that Lorem Ipsum is that hu</h3>
                <img class="job-terms-image d-block mx-auto" src="../assets/Job Detail (1).png" alt="user">
                <p class="job-terms-text mt-14 text-center font-weight-medium">Design comps, layouts, wireframes—will your clients accept that you go about
                    things the facile way? Authorities in our business will tell in no
                    uncertain terms that Lorem Ipsum is that huge, huge no no to forswear forever.</p>
                <p class="job-terms-text text-center font-weight-medium"> The toppings you may chose for that TV dinner pizza slice when you forgot to
                    shop
                    for foods, the paint you
                    may slap on your face to impress the new boss is your business. But what about your daily bread? Not so
                    fast, I'd say, there are some
                    redeeming factors in favor of greeking text, as its use is merely the symptom of a worse problem to take
                    into consideration.</p>
                <p class="job-terms-text text-center font-weight-medium"> Not so fast, I'd say, there are some redeeming factors in favor of greeking text,
                    as its use is merely the
                    symptom of a worse problem to take into consideration. </p>
                <p class="job-terms-text mb-14 text-center font-weight-medium"> Design comps, layouts, wireframes—will your clients accept that you go
                    about
                    things the facile way? Authorities in our business will tell in
                    no uncertain terms that Lorem Ipsum is that huge, huge no no to forswear forever.</p>
            </div>
            <div class="job-terms">
                <img class="job-terms-image d-block mx-auto" src="../assets/Job Detail (2).png" alt="user">
                <p class="job-terms-text mt-14 text-center font-weight-medium">Design comps, layouts, wireframes—will your clients accept that you go about
                    things the facile way? Authorities in our business will tell in no
                    uncertain terms that Lorem Ipsum is that huge, huge no no to forswear forever.</p>
                <p class="job-terms-text text-center font-weight-medium"> The toppings you may chose for that TV dinner pizza slice when you forgot to
                    shop
                    for foods, the paint you
                    may slap on your face to impress the new boss is your business. But what about your daily bread? Not so
                    fast, I'd say, there are some
                    redeeming factors in favor of greeking text, as its use is merely the symptom of a worse problem to take
                    into consideration.</p>
                <p class="job-terms-text text-center font-weight-medium"> Not so fast, I'd say, there are some redeeming factors in favor of greeking text,
                    as its use is merely the
                    symptom of a worse problem to take into consideration. </p>
                <p class="job-terms-text text-center font-weight-medium"> Design comps, layouts, wireframes—will your clients accept that you go about
                    things the facile way? Authorities in our business will tell in
                    no uncertain terms that Lorem Ipsum is that huge, huge no no to forswear forever.</p>
            </div>
        </v-container>
    </div>
</template>

<script>
export default {
    name: "JobDetail",
    data() {
        return {
        //   
        }
    }
}

</script>
<style>
/* style is here */
.job-detail-title {
    margin: 30px 100px 50px 100px;
    font-family: 'Oswald';
    font-size: 82px;
    line-height: 100px;
    color: #111827;
}

.job-detail-text {
    font-family: 'Poppins';
    font-size: 16px;
    line-height: 25px;
    text-align: center;
    color: #222222;
}

.job-terms-title {
    font-family: 'Poppins';
    font-size: 28px;
    line-height: 40px;
    color: #222222;
}

.job-terms-image {
    width: 1000px;
}

.job-terms-text {
    font-family: 'Poppins';
    font-size: 16px;
    line-height: 25px;
    color: #222222;
}

/* media queries is here */
@media screen and (min-width:1900px) {
    #job-detail {
        margin-left: 330px;
        margin-right: 330px;
    }
   
}

@media screen and (max-width:1260px) {
    .job-terms-image {
        width: 750px;
    }
}

@media screen and (max-width:960px) {
    .job-detail-title {
        margin: 30px 40px 50px 40px;
        font-size: 60px;
        line-height: 80px;
    }

    .job-terms-image {
        width: 700px;
    }
}

@media screen and (max-width:800px) {
    .job-terms-image {
        width: 600px;
    }
    
}

@media screen and (max-width:660px) {
    .job-detail-title {
        margin: 30px 10px 50px 10px;
        font-size: 45px;
        line-height: 60px;
    }

    .job-terms-image {
        width: 500px;
    }
}

@media screen and (max-width:550px) {
    .job-terms-image {
        width: 400px;
        height: 200px;
    }
}

@media screen and (max-width:450px) {
    .job-terms-image {
        width: 300px;
        height: 150px;
    }
   
}</style>
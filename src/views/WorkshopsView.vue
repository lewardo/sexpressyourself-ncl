<script setup>
import PageTitle from '@/components/PageTitle.vue'

import CarouselWrapper from '@/components/CarouselWrapper.vue'
import CarouselSlide from '@/components/CarouselSlide.vue'
</script>

<template>
    <PageTitle title="Workshops" :schedule="true" />

    <div class="content">
        <CarouselWrapper>
            <CarouselSlide name="one" prev="three" next="two">
                <div class="card">
                    <div class="img">
                        <img src="@/assets/img/persons/dami.jpg" alt="Dami Fawehinmi">
                    </div>
                    <div class="text"> 
                        <span>Collage Workshop</span>
                        <br>
                        Join Journals Of Dami (Dami Fawehinmi, any pronouns) as they lead a group workshop on intersectional sex and support through chronic illnesses such as endometriosis through the Black and Queer lens. 
                        This workshop will last 1 hour and be immersive, utilising a variety of artistic materials to collage your experiences through sex, mental and physical well-being, as well as learn how to support yourself and others through this.
                    </div>
                </div>    
            </CarouselSlide>
            <CarouselSlide name="two" prev="one" next="three"> two </CarouselSlide>
            <CarouselSlide name="three" prev="two" next="one"> three </CarouselSlide>
        </CarouselWrapper>
    </div>
</template>

<style scoped>
@import '@/assets/view.css';
.content {
    width: 90%;
}

.card {
    width: 100%;
    height: 100%;
    display: flex;
    color: #fff;
    font-size: 2vh;
    background-color: #1a60d688;
}

.img {
    height: 100%;
}

.img img {
    height: 100%;
}

.text {
    padding: 2.5vh;
}

.workshop-name, .text span {
    font-size: 3vh;
    font-weight: bolder;
}

.info {
    margin-left: auto;
}

hr {
    border: 1px solid #000;
    margin: 0 0 1em;
}

@media screen and (max-aspect-ratio: 5/4) {
    .img {
        display: none;
    }
}
</style>

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
                    <div class="workshop-img">
                        <img src="@/assets/img/persons/dami.jpg" alt="Dami Fawehinmi">
                    </div>
                    <div class="workshop-info"> 
                        <div class="workshop-name">Collage Workshop</div>
                        <div class="workshop-desc">
                            Join Journals Of Dami (Dami Fawehinmi, any pronouns) as they lead a group workshop on intersectional sex and support through chronic illnesses such as endometriosis through the Black and Queer lens. 
                            This workshop will last 1 hour and be immersive, utilising a variety of artistic materials to collage your experiences through sex, mental and physical well-being, as well as learn how to support yourself and others through this.
                        </div>
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

.workshop-img {
    height: 100%;
}

.workshop-img img {
    height: 100%;
}

.workshop-info {
    padding: 2.5vh;
}

.workshop-name {
    font-size: 3vh;
    font-weight: bolder;
}

@media screen and (max-aspect-ratio: 5/4) {
    .workshop-img {
        display: none;
    }
}
</style>

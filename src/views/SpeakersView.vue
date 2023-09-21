<script setup>
import PageTitle from '@/components/PageTitle.vue'

import CarouselWrapper from '@/components/CarouselWrapper.vue'
import CarouselSlide from '@/components/CarouselSlide.vue'
</script>

<template>
    <PageTitle title="Speakers" :schedule="true" />

    <div class="content">
        <CarouselWrapper>
            <CarouselSlide name="collage-speaker" prev="burlesque-speaker" next="tote-speaker">
                <div class="card">
                    <img src="@/assets/img/persons/marina.jpg" alt="Dami Fawehinmi" />
                    <div class="speaker-info">
                        <div class="speaker-name">Marina Carvalho</div>
                        <div class="speaker-desc">
                            Sex therapist with a PhD Course in Human Sexuality (University of Porto
                            — UP), M.A. in Clinical Psychology (Pontifical Catholic University of
                            São Paulo — PUC-SP) and a Post Graduate Course in Clinical Sexology (The
                            Portuguese Institute of Psychology and other Sciences — INSPSIC). My
                            studies focus on sexual pleasure, sexual difficulties, sexual diversity
                            (LGBTQIA+) and reflections on being men and women in contemporary times.
                            I work individually with adults, online or face-to-face in Newcastle.
                            <br />
                            <a href="https://myurbanangel.co.uk/therapist/marina-carvalho/">
                                Urban Angel Clinic
                            </a>
                        </div>
                    </div>
                </div>
            </CarouselSlide>
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

img {
    height: 100%;
}

.speaker-info {
    padding: 2.5vh;
}

.speaker-name {
    font-size: 3vh;
    font-weight: bolder;
}

@media screen and (max-aspect-ratio: 5/4) {
    img {
        display: none;
    }
}
</style>

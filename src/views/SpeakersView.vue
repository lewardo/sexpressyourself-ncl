<script setup>
import PageTitle from '@/components/PageTitle.vue'

import CarouselWrapper from '@/components/CarouselWrapper.vue'
import CarouselSlide from '@/components/CarouselSlide.vue'
</script>

<template>
    <PageTitle title="Speakers" :schedule="true" />

    <div class="content">
        <CarouselWrapper>
            <CarouselSlide name="echo" prev="temp-2" next="carvalho">
                <div class="card">
                    <div class="speaker-img img-eva">
                        <img src="@/assets/img/persons/eva.jpg" alt="Eva Echo" />
                    </div>
                    <div class="speaker-info">
                        <div class="speaker-name">Eva Echo</div>
                        <div class="speaker-desc">
                            <div>
                                Eva Echo (she/they) is an activist, writer and public speaker with 
                                a focus on transgender rights and mental health. She uses her own 
                                experiences to shed light on what it is to be transgender and to 
                                challenge the obstacles which gender diverse people face within today's 
                                society. Most notably, Eva took legal action against NHS England in the 
                                High Court to challenge the unlawful waiting times for trans patients. 
                                She won the DIVA Award for Unsung Hero of the Year 2022 and was named 
                                on the DIVA Power List for 2022 and 2023. She was also named 19th in the 
                                Pride Power List 2023. Eva won Trans in the City's Trans Community Champion 
                                award for 2022 and went on to become of their Directors. Eva is also Director 
                                of Innovation at Birmingham Pride, an ambassador for the charity Diversity 
                                Role Models and sits on the Crown Prosecution Service's hate crime panel. 
                                As of 2023, Eva's story was included in the Science Museum's permanent 
                                "Who Am I?" gallery, which aims to promote diversity and education to all 
                                current and future generations.
                            </div>
                        </div>
                    </div>
                </div>
            </CarouselSlide>
            <CarouselSlide name="carvalho" prev="echo" next="etherson">
                <div class="card">
                    <div class="speaker-img">
                        <img src="@/assets/img/persons/marina.png" alt="Marina Carvalho"/>
                    </div>
                    <div class="speaker-info">
                        <div class="speaker-name">Marina Carvalho</div>
                        <div class="speaker-desc">
                            <div>
                                Sex therapist with a PhD Course in Human Sexuality (University of
                                Porto — UP), M.A. in Clinical Psychology (Pontifical Catholic
                                University of São Paulo — PUC-SP) and a Post Graduate Course in
                                Clinical Sexology (The Portuguese Institute of Psychology and other
                                Sciences — INSPSIC). My studies focus on sexual pleasure, sexual
                                difficulties, sexual diversity (LGBTQIA+) and reflections on being
                                men and women in contemporary times. I work individually with
                                adults, online or face-to-face in Newcastle.
                                <br />
                                <a href="https://myurbanangel.co.uk/therapist/marina-carvalho/">
                                    Urban Angel Clinic
                                </a>
                            </div>
                        </div>
                    </div>
                </div>
            </CarouselSlide>
            <CarouselSlide name="etherson" prev="carvalho" next="sheinman">
                <div class="card">
                    <div class="speaker-img">
                        <img src="@/assets/img/persons/lisa.png" alt="Lisa Etherson"/>
                    </div>
                    <div class="speaker-info">
                        <div class="speaker-name">Lisa Etherson</div>
                        <div class="speaker-desc">
                            <div>
                                Lisa Etherson is a PhD researcher, currently exploring shame. As a
                                Psychosexual Therapist she has a busy private practice with a
                                special interest in porn use and compulsive sexual behaviour. She
                                has over 20 years' experience of working with people
                                therapeutically, usually finding herself discussing the most taboo
                                of subjects. She is a keen advocate for accurate, timely sex
                                education.
                            </div>
                        </div>
                    </div>
                </div>
            </CarouselSlide>
            <CarouselSlide name="sheinman" prev="etherson" next="temp-1">
                <div class="card">
                    <div class="speaker-img">
                        <img src="@/assets/img/persons/gem.png" alt="Gem Sheinman"/>
                    </div>
                    <div class="speaker-info">
                        <div class="speaker-name">Gem Sheinman</div>
                        <div class="speaker-desc">
                            <div>
                                Gem Sheinman is a qualified Psychotherapeutic Counsellor who practises 
                                person centred and transactional analysis therapy. Gem is an a LGBTQ+ 
                                identified therapist, and specialises in working with Queer people and 
                                couples to negotiate relationships, lives and family dynamics. Our 
                                intersecting identities impact our lived experience, and deepening 
                                self-understanding towards a fuller, more authentic and enriching life.
                            </div>
                        </div>
                    </div>
                </div>
            </CarouselSlide>
            <CarouselSlide name="temp-1" prev="sheinman" next="temp-2">
                <div class="card">
                    <div class="speaker-img patched">
                        <img src="@/assets/img/logo_full_wide.png" alt="Sexpression Newcastle Logo" />
                    </div>
                    <div class="speaker-info">
                        <div class="speaker-name">To be Announced</div>
                        <div class="speaker-desc">
                            <div>
                                Certain speakers have not yet been announced publicly, stay tuned for any updates!
                            </div>
                        </div>
                    </div>
                </div>
            </CarouselSlide>
            <CarouselSlide name="temp-2" prev="temp-1" next="temp-3">
                <div class="card">
                    <div class="speaker-img patched">
                        <img src="@/assets/img/logo_full_wide.png" alt="Sexpression Newcastle Logo" />
                    </div>
                    <div class="speaker-info">
                        <div class="speaker-name">To be Announced</div>
                        <div class="speaker-desc">
                            <div>
                                Certain speakers have not yet been announced publicly, stay tuned for any updates!
                            </div>
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
    font-size: 2.5vh;
    border-radius: 24px;
    background-color: #1a60d688;
    scrollbar-width: none;
    -ms-overflow-style: none;
}

.card::-webkit-scrollbar {
    display: none;
}

.speaker-img {
    height: 100%;
    min-width: 40%;
    overflow: hidden;
    z-index: 1;
    background-color: white;
}

.speaker-img.patched {
    width: 40%;
}

img {
    height: 100%;
    position: relative;
    left: 50%;
    transform: translateX(-50%);
}

.img-eva {
    background-image: url('@/assets/img/persons/eva-og.jpg');
    background-position: top;
    background-size: cover;
}

.img-eva img {
    display: none;
}

@media screen and (max-aspect-ratio: 4/5) {
    .img-eva img {
        display: block;
    }
}

.speaker-info {
    padding: 2.5vh;
}

.speaker-info {
    overflow: scroll;
    scrollbar-width: none;
    -ms-overflow-style: none;
}

.speaker-info::-webkit-scrollbar {
    display: none;
}

.speaker-desc div::after {
    content: '';
    display: block;
    width: 100%;
    height: 10%;
    position: absolute;
    bottom: 0;
    left: 0;
    background: linear-gradient(0deg, #4387e9ff, #4387e900);
}

.speaker-name {
    font-size: 3vh;
    font-weight: bolder;
}

@media screen and (max-aspect-ratio: 4/5) {
    .card {
        flex-direction: column;
        overflow: scroll;
        scrollbar-width: none;
        -ms-overflow-style: none;
    }

    .card::-webkit-scrollbar {
        display: none;
    }

    .speaker-info {
        overflow: visible;
    }

    .speaker-img, .speaker-img.patched {
        width: 100%;
        aspect-ratio: 16 / 9;
        height: auto;
        overflow: visible;
    }

    .speaker-img img {
        width: 100%;
        overflow: visible;
        position: static;
        transform: none;
    }
}
</style>

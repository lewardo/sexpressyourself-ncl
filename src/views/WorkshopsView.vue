<script setup>
import PageTitle from '@/components/PageTitle.vue'

import CarouselWrapper from '@/components/CarouselWrapper.vue'
import CarouselSlide from '@/components/CarouselSlide.vue'
</script>

<template>
    <PageTitle title="Workshops" :schedule="true" />

    <div class="content">
        <CarouselWrapper>
            <CarouselSlide name="collage-workshop" prev="burlesque-workshop" next="tote-workshop">
                <div class="card">
                    <img src="@/assets/img/persons/dami.jpg" alt="Dami Fawehinmi">
                    <div class="workshop-info"> 
                        <div class="workshop-name">Collage Workshop</div>
                        <div class="workshop-desc">
                            Join Journals Of Dami (Dami Fawehinmi, any pronouns) as they lead a group workshop on intersectional sex and support through chronic illnesses such as endometriosis through the Black and Queer lens. 
                            This workshop will last 1 hour and be immersive, utilising a variety of artistic materials to collage your experiences through sex, mental and physical well-being, as well as learn how to support yourself and others through this.
                        </div>
                    </div>
                </div>    
            </CarouselSlide>
            <CarouselSlide name="tote-workshop" prev="collage-workshop" next="cupcake-workshop">
                <div class="card">
                    <!-- <img src="@/assets/img/persons/dami.jpg" alt="Dami Fawehinmi"> -->
                    <div class="workshop-info"> 
                        <div class="workshop-name">Tote Bag Workshop</div>
                        <div class="workshop-desc">                      
                            Hone in to your creative side and really (s)express yourself with this tote bag designing and decorating workshop. We'll have sex-positive instructions on how to make your very own vulva tote (you can even add labels if you want an extra educational twist), but you can also freely explore your own tote bag ideas! Come along to find out what you can create.
                        </div>
                    </div>
                </div>    
            </CarouselSlide>
            <CarouselSlide name="cupcake-workshop" prev="tote-workshop" next="drawing-workshop">
                <div class="card">
                    <!-- <img src="@/assets/img/persons/dami.jpg" alt="Dami Fawehinmi"> -->
                    <div class="workshop-info"> 
                        <div class="workshop-name">Cupcake Decorating Workshop</div>
                        <div class="workshop-desc">
                            Cupcakes... clitcakes... a whole lotta cakes! In this workshop, we'll be letting you loose with fondant, icing, and lots of other goodies - so you can design and make (and eventually, eat) your own sex-positive cupcakes. Our committee will be having a go at the Netlflix-inspired vulva cupcakes, but feel free to be inspired and be creative!
                        </div>
                    </div>
                </div>    
            </CarouselSlide>
            <CarouselSlide name="drawing-workshop" prev="cupcake-workshop" next="burlesque-workshop">
                <div class="card">
                    <!-- <img src="@/assets/img/persons/dami.jpg" alt="Dami Fawehinmi"> -->
                    <div class="workshop-info"> 
                        <div class="workshop-name">Life Drawing Workshop</div>
                        <div class="workshop-desc">
                            Come and try your hand at life drawing in this safe, positive environment. Our model Rikki will be clothed, he is absolutely lovely, and the session will be guided by one of our committee members. Please note that phones will be kept in a box throughout this workshop, to help with the safe atmosphere.
                        </div>
                    </div>
                </div>    
            </CarouselSlide>
            <CarouselSlide name="burlesque-workshop" prev="drawing-workshop" next="collage-workshop">
                <div class="card">
                    <img src="@/assets/img/persons/vintage.jpg" alt="Dami Fawehinmi">
                    <div class="workshop-info"> 
                        <div class="workshop-name">Burleqsue Dance Workshop</div>
                        <div class="workshop-desc">
                            ROLL UP ROLL UP!!!!! do you love the beauty of burlesque?
                            Want to unleash your inner sparkle, build confidence and learn something new? Here at House of Trixie Blue we have developed a 60mins beginner's burlesque workshop that will introduce you to burlesque in a relaxed and friendly manner with a bit of sass and class. Learn the beauty and the techniques of the tease, from peeling, posing and much much more.
                            Taught by our professional burlesque performers and PGCE qualified teachers, who uphold our ethos of accessible and inclusive burlesque, you shall be sure to develop your new skills in a supportive atmosphere. No experience required and no nudity. 18+ all bodies & genders welcome.
                            (please wear comfortable shoes and clothing, such as leggings and a tshirt - whatever works for you)                        
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

.workshop-info {
    padding: 2.5vh;
}

.workshop-name {
    font-size: 3vh;
    font-weight: bolder;
}

@media screen and (max-aspect-ratio: 5/4) {
    img {
        display: none;
    }
}
</style>

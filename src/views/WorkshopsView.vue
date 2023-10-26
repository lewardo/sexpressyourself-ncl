<script setup>
import PageTitle from '@/components/PageTitle.vue'

import CarouselWrapper from '@/components/CarouselWrapper.vue'
import CarouselSlide from '@/components/CarouselSlide.vue'
</script>

<template>
    <PageTitle title="Workshops" :schedule="true" />

    <div class="content">
        <CarouselWrapper>
            <CarouselSlide name="collage-workshop" prev="dragsoc-workshop" next="burlesque-workshop">
                <div class="card">
                    <div class="workshop-img">
                        <img src="@/assets/img/persons/dami.png" alt="Dami Fawehinmi"/>
                    </div>
                    <div class="workshop-info">
                        <div class="workshop-name">Collage Workshop</div>
                        <div class="workshop-desc">
                            <div>
                                Join Journals Of Dami (Dami Fawehinmi, any pronouns) as they lead a
                                group workshop on intersectional sex and support through chronic
                                illnesses such as endometriosis through the Black and Queer lens.
                                This workshop will last 1 hour and be immersive, utilising a variety
                                of artistic materials to collage your experiences through sex,
                                mental and physical well-being, as well as learn how to support
                                yourself and others through this.
                            </div>
                        </div>
                    </div>
                </div>
            </CarouselSlide>
            <CarouselSlide name="burlesque-workshop" prev="collage-workshop" next="meditation-workshop">
                <div class="card">
                    <div class="workshop-img">
                        <img src="@/assets/img/persons/vintage.png" alt="Trixie Blue" />
                    </div>
                    <div class="workshop-info">
                        <div class="workshop-name">Burleqsue Dance Workshop</div>
                        <div class="workshop-desc">
                            <div>
                                ROLL UP ROLL UP!!!!! do you love the beauty of burlesque? Want to
                                unleash your inner sparkle, build confidence and learn something
                                new? Here at House of Trixie Blue we have developed a 60mins
                                beginner's burlesque workshop that will introduce you to burlesque
                                in a relaxed and friendly manner with a bit of sass and class. Learn
                                the beauty and the techniques of the tease, from peeling, posing and
                                much much more. Taught by our professional burlesque performers and
                                PGCE qualified teachers, who uphold our ethos of accessible and
                                inclusive burlesque, you shall be sure to develop your new skills in
                                a supportive atmosphere. No experience required and no nudity. 18+
                                all bodies & genders welcome. (please wear comfortable shoes and
                                clothing, such as leggings and a tshirt - whatever works for you)
                            </div>
                        </div>
                    </div>
                </div>
            </CarouselSlide>
            <CarouselSlide name="meditation-workshop" prev="burlesque-workshop" next="freewriting-workshop">
                <div class="card">
                    <div class="workshop-img">
                        <img src="@/assets/img/persons/meditation.png" alt="A Meditation Group" />
                    </div>
                    <div class="workshop-info">
                        <div class="workshop-name">The Way My Body Feels</div>
                        <div class="workshop-desc">
                            <div>
                                An interactive workshop led by artist Olivia Turner and Classical archaeologist 
                                Sally Waite, to consider the links between objects, art, and medicine. Through 
                                meditation, votive object handling, and art making we will explore the different 
                                ways we 'imagine our insides'. The Way My Body Feels demonstrates the transformative 
                                role ancient objects can play in learning about the body and in particular, the 
                                body in medicine.
                            </div>
                        </div>
                    </div>
                </div>
            </CarouselSlide>
            <CarouselSlide name="freewriting-workshop" prev="meditation-workshop" next="tote-workshop">
                <div class="card">
                    <div class="workshop-img">
                        <img src="@/assets/img/persons/stamper.jpg" alt="Isaac Stamper" />
                    </div>
                    <div class="workshop-info">
                        <div class="workshop-name">Freewriting Workshop</div>
                        <div class="workshop-desc">
                            <div>
                                Isaac Stamper (he/him) will be running an inclusive creative free-writing session on expression 
                                and independence. All are welcome! No prior practice required, it's just a "give-it-a-go" and 
                                fun writing workshop. Nice chill vibes included, we want to promote a safe space for free-writing :)
                            </div>
                        </div>
                    </div>
                </div>
            </CarouselSlide>
            <CarouselSlide name="tote-workshop" prev="freewriting-workshop" next="cupcake-workshop">
                <div class="card">
                    <div class="workshop-img">
                        <img src="@/assets/img/logo_full_wide.png" alt="Sexpression Newcastle Logo" />
                    </div>
                    <div class="workshop-info">
                        <div class="workshop-name">Tote Bag Workshop</div>
                        <div class="workshop-desc">
                            <div>
                                Hone in to your creative side and really (s)express yourself with
                                this tote bag designing and decorating workshop. We'll have
                                sex-positive instructions on how to make your very own vulva tote
                                (you can even add labels if you want an extra educational twist),
                                but you can also freely explore your own tote bag ideas! Come along
                                to find out what you can create.
                            </div>
                        </div>
                    </div>
                </div>
            </CarouselSlide>
            <CarouselSlide name="cupcake-workshop" prev="tote-workshop" next="drawing-workshop">
                <div class="card">
                    <div class="workshop-img">
                        <img src="@/assets/img/logo_full_wide.png" alt="Sexpression Newcastle Logo" />
                    </div>
                    <div class="workshop-info">
                        <div class="workshop-name">Cupcake Decorating Workshop</div>
                        <div class="workshop-desc">
                            <div>
                                Cupcakes... clitcakes... a whole lotta cakes! In this workshop,
                                we'll be letting you loose with fondant, icing, and lots of other
                                goodies - so you can design and make (and eventually, eat) your own
                                sex-positive cupcakes. Our committee will be having a go at the
                                Netlflix-inspired vulva cupcakes, but feel free to be inspired and
                                be creative!
                            </div>
                        </div>
                    </div>
                </div>
            </CarouselSlide>
            <CarouselSlide name="drawing-workshop" prev="cupcake-workshop" next="bounce-workshop">
                <div class="card">
                    <div class="workshop-img">
                        <img src="@/assets/img/logo_full_wide.png" alt="Sexpression Newcastle Logo" />
                    </div>
                    <div class="workshop-info">
                        <div class="workshop-name">Life Drawing Workshop</div>
                        <div class="workshop-desc">
                            <div>
                                Come and try your hand at life drawing in this safe, positive
                                environment. Our model Rikki will be clothed, he is absolutely
                                lovely, and the session will be guided by one of our committee
                                members. Please note that phones will be kept in a box throughout
                                this workshop, to help with the safe atmosphere.
                            </div>
                        </div>
                    </div>
                </div>
            </CarouselSlide>
            <CarouselSlide name="bounce-workshop" prev="drawing-workshop" next="mythbuster-workshop">
                <div class="card">
                    <div class="workshop-img">
                        <img src="@/assets/img/persons/azula.png" alt="Azula Bandit" />
                    </div>
                    <div class="workshop-info">
                        <div class="workshop-name">Bounce with Bandit</div>
                        <div class="workshop-desc">
                            <div>
                                Hey there, booty shakers! Welcome to Bounce with Bandit, where we're all 
                                about embracing the art of Booty Bouncing. It all started back in 2017 
                                when Azula Bandit decided it was time to create a space where all Womxn 
                                could come together, let loose, and dance like nobody's watching.
                                Azula's the brain (and the booty) behind the operation. Their passion for 
                                dance and a deep desire to help people feel empowered and expressive led to 
                                the birth of Bounce with Bandit. We're not just about dance but about 
                                celebrating confidence and sensuality.
                                Bounce with Bandit is a judgment-free zone. Everyone is welcome whether 
                                you're a seasoned dancer or a total newbie. We're all about loving the skin 
                                you're in.
                                Confidence is Key: Beyond the dance moves, our classes are confidence-boosting 
                                experiences. We're here to remind you that your body is incredible, and 
                                expressing yourself is beautiful.
                            </div>
                        </div>
                    </div>
                </div>
            </CarouselSlide>
            <CarouselSlide name="mythbuster-workshop" prev="bounce-workshop" next="dragsoc-workshop">
                <div class="card">
                    <div class="workshop-img patched">
                        <img src="@/assets/img/logo_full_wide.png" alt="Sexpression Newcastle Logo" />
                    </div>
                    <div class="workshop-info">
                        <div class="workshop-name">Embarassing (female) bodies: busting the myths</div>
                        <div class="workshop-desc">
                            <div>
                                This workshop, run by a Clinical Nurse Specialist, will cover abnormal vaginal 
                                discharge and pain, development, appearances and examination of the external 
                                genitalia, and myths regarding HPV and cervical screening.
                            </div>
                        </div>
                    </div>
                </div>
            </CarouselSlide>
            <CarouselSlide name="dragsoc-workshop" prev="mythbuster-workshop" next="collage-workshop">
                <div class="card">
                    <div class="workshop-img patched">
                        <img src="@/assets/img/persons/dragsoc.jpg" alt="Sexpression Newcastle Logo" />
                    </div>
                    <div class="workshop-info">
                        <div class="workshop-name">The Cocalily and Vendetta Vedele</div>
                        <div class="workshop-desc">
                            <div>
                                Join Newcastle University Drag Society's The Cocalily and Vendetta Vedele as 
                                they lead a 'get ready with me' workshop, and talk about all things sexpressing 
                                yourself, including gender identity and fetishisation.
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

.workshop-img {
    height: 100%;
    min-width: 40%;
    overflow: hidden;
    z-index: 1;
    background-color: white;
}

.workshop-img.patched {
    width: 40%;
}

img {
    height: 100%;
    position: relative;
    left: 50%;
    transform: translateX(-50%);
}

.workshop-info {
    padding: 2.5vh;
}

.workshop-info {
    overflow: scroll;
    scrollbar-width: none;
    -ms-overflow-style: none;
}

.workshop-info::-webkit-scrollbar {
    display: none;
}

.workshop-desc div::after {
    content: '';
    display: block;
    width: 100%;
    height: 10%;
    position: absolute;
    bottom: 0;
    left: 0;
    background: linear-gradient(0deg, #4387e9ff, #4387e900);
}

.workshop-name {
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

    .workshop-info {
        overflow: visible;
    }

    .workshop-img, .workshop-img.patched {
        width: 100%;
        aspect-ratio: 16 / 9;
        height: auto;
        overflow: visible;
    }

    .workshop-img img {
        width: 100%;
        overflow: visible;
        position: static;
        height: auto;
        transform: none;
    }
}
</style>

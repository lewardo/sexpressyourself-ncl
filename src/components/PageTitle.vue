<script setup>
import { Countdown } from 'vue3-flip-countdown'

defineProps({
    title: {
        type: String,
        required: true
    },
    subtitle: {
        type: Boolean,
        required: false,
        default: true
    },
    schedule: {
        type: Boolean,
        required: false,
        default: false
    }
})
</script>

<template>
    <div class="title">
        <a href="/">
            <img
                src="@/assets/img/title.png"
                class="title-img"
                alt="sexpress yourself conference banner"
                draggable="false" />
        </a>
        <div v-if="subtitle" class="subtitle">
            <span>{{ title }}</span>
            <a v-if="schedule" href="/assets/schedule.pdf">
                <span class="download-schedule">Schedule</span>
            </a>
        </div>
        <Countdown v-else deadline="2023-11-04 00:00:00" 
                    countdownSize="8vmin"
                    labelSize="2vmin"
                    mainColor="#fff" 
                    secondFlipColor="#fff" 
                    mainFlipBackgroundColor="#004aad" 
                    secondFlipBackgroundColor="#1a60d6" 
        />
        <br />
    </div>
</template>

<style scoped>
.title {
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.title > a {
    max-height: 30vh;
    display: flex;
    place-items: center;
    justify-content: center;
}

.title-img {
    height: 100%;
}


.flip-clock {
    /* align-self: flex-start; */
    /* margin: 2vh auto; */
    padding: 1vh 0 0 0;
}

@media screen and (max-aspect-ratio: 5/4) {
    .title-img {
        max-width: 80vw;
    }
}

.subtitle {
    width: 100%;
    line-height: min(6vh, 8vw);
    font-size: min(3vh, 4vw);
    display: flex;
    justify-content: center;
    margin: 1vh 0;
}

.subtitle > span {
    color: #fff;
    background-color: #0f0a62;
    padding: 0 min(24px, 5vw);
    border-radius: 100vw;
    box-shadow: 0 0 4px 0 #000;
}

.subtitle a {
    color: #fff;
    background-color: #ff3131;
    text-decoration: none;
    padding: 0 min(24px, 5vw);
    margin: 0 0 0 12px;
    border-radius: 100vw;
    box-shadow: 0 0 4px 0 #000;
}

.subtitle a:active {
    box-shadow: none;
}
</style>

<script setup>
import { Countdown } from 'vue3-flip-countdown'
import PageTitle from '@/components/PageTitle.vue'
</script>

<template>
    <PageTitle title="Home" :subtitle="false" />

    <div class="content">
        <br />
        <Countdown  deadline="2023-11-04 00:00:00" 
                    countdownSize="8vmin"
                    mainColor="#fff" 
                    secondFlipColor="#fff" 
                    mainFlipBackgroundColor="#004aad" 
                    secondFlipBackgroundColor="#1a60d6" />
        
        <br />
        <div class="msg">
            <span> 
                Join us for NC@NCL, 
                <span style="text-shadow: 0 0 8px #9b01ff;">Sexpression</span> 
                National Conference 2023
            </span>
            <br />
            <span> Sat 4th and Sun 5th November 2023 </span>
        </div>
    </div>
</template>

<style scoped>
@import '@/assets/view.css';

.content {
    font-size: min(3vh, 6vw);
    width: 90%;
    flex-grow: 1;
    margin-top: 1vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
}

.content .flip-clock {
    align-self: flex-start;
    margin: 2vh auto;
}

.content hr {
    border: 1px solid #000;
}

.content .msg {
    font-size: min(4vw, 4vh);
    /* flex-grow: 1;
    display: flex;
    flex-direction: column;
    justify-content: center; */
}
</style>

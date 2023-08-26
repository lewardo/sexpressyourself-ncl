<script setup>
import { Countdown } from 'vue3-flip-countdown'
import PageTitle from '@/components/PageTitle.vue'
</script>

<template>
    <PageTitle title="Home" :subtitle="false" />

    <div class="content">
        <div class="msg">
            <span> 
                Join us for NC@NCL, Sexpression National Conference 2023
            </span>
            <span> 
                Sat 4th and Sun 5th November 2023 
            </span>
        </div>
    </div>

    <Countdown deadline="2023-11-04 10:00:00" 
                   countdownSize="10vmin"
                   labelSize="2.5vmin"
                   mainColor="#fff" 
                   secondFlipColor="#fff" 
                   mainFlipBackgroundColor="#1a60d6" 
                   secondFlipBackgroundColor="#1a60d6" 
        />
</template>

<style scoped>
@import '@/assets/view.css';

.content {
    font-size: min(3vh, 6vw);
    width: 90%;
    flex-grow: 1;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    text-align: center;
    background-color: #1a60d688;
    border-radius: 24px;
    margin-bottom: 2vh;
}

.content hr {
    border: 1px solid #000;
}

.content .msg {
    font-size: min(6vw, 4vh);
    color: #fff;
    flex-grow: 1;
    display: flex;
    flex-direction: column;
    justify-content: center;
}
</style>

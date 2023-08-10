<script setup>
import PageTitle from '@/components/PageTitle.vue'
</script>

<template>
    <PageTitle title="Home" :subtitle="false" />

    <div class="content">
        <div class="msg">
            <span> 
                Join us for NC@NCL, Sexpression National Conference 2023
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

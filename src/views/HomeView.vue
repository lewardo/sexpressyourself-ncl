<script setup>
import PageTitle from '@/components/PageTitle.vue'
</script>

<template>
    <PageTitle title="Home" :subtitle="false" />

    <div class="content">
        <div class="msg">
            <span> Join us for National Conference 2023 </span>
            <br />
            <span> NC@NCL </span>
            <hr />
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
    justify-content: center;
    text-align: center;
    background-color: #00000020;
    border-radius: 24px;
}

.content hr {
    border: 1px solid #000;
}
</style>

<script setup>
import PageTitle from "@/components/PageTitle.vue"
</script>

<template>
    <PageTitle title="About" />

    <div class="content">
        <div class="info">
            Sexpression:&#8203;Newcastle form part of the UK-wide sex-education charity <a href="https://sexpression.org.uk/">Sexpression:UK</a>. We are a UK-based, near-peer charity who run comprehensive RSE in the community, with the goal of empowering young people to make decisions about relationships and sex.
            This year, Newcastle are the nominated hosts of the Sexpression:UK National Conference 2023, on the 4th and 5th of November, with the theme '(S)express Yourself'. This will provide opportunities for sex-positive education and expression for university students and adults. We hope to welcome up to 120 attendees, made up of Sexpression members and alumni, as well as members of the general public interested in sexual health.
        </div>
    </div>
</template>

<style scoped>
@import "@/assets/view.css";

.content {
    width: 90%;
    font-size: 2.5vmin;
    color: #fff;
    border-radius: 24px;
    overflow: hidden;
    background: #1a60d688;
    padding: 1.5vh;
    text-align: center;
    display: grid;
    place-items: center;
}

</style>

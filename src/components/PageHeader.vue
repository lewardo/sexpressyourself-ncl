<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
    <nav class="header">
        <RouterLink to="/speakers">
            <span>Speakers&nbsp;</span>
            <i class="fa fa-user"></i>
        </RouterLink>
        <RouterLink to="/workshops">
            <span>Workshops&nbsp;</span>
            <i class="fa fa-calendar"></i>
        </RouterLink>
        <RouterLink to="/about">
            <span>About&nbsp;</span>
            <i class="fa fa-question"></i>
        </RouterLink>
        <RouterLink to="/contact">
            <span>Contact&nbsp;</span>
            <i class="fa fa-envelope"></i>
        </RouterLink>
    </nav>
</template>

<style scoped>
    .header {
        width: 100%;
        height: 10%;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-around;
    }

    .header > * {
        line-height: min(6vh, 8vw);
        font-size: min(3vh, 4vw);
        text-align: center;
        min-width: 20vw;
        color: #fff;
        background-color: var(--colour-emphasis);
        text-decoration: none;
        border-radius: 3vh;
        cursor: pointer;
        padding: 0 10px;
    }

    .header > * i {
        font-weight: light;
    }

    @media screen and ( max-aspect-ratio: 1/1 ) {
        .header > * {
            min-width: min(6vh, 8vw);
        }

        .header > * span {
            display: none;
        }
    }
</style>
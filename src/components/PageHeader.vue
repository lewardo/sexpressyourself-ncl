<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
    <nav class="header">
        <RouterLink class="router-link" to="/speakers">
            <span>Speakers&nbsp;</span>
            <i class="fa fa-user"></i>
        </RouterLink>
        <RouterLink class="router-link" to="/workshops">
            <span>Workshops&nbsp;</span>
            <i class="fa fa-calendar"></i>
        </RouterLink>
        <RouterLink class="router-link" to="/about">
            <span>About&nbsp;</span>
            <i class="fa fa-question"></i>
        </RouterLink>
        <RouterLink class="router-link" to="/contact">
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

    .header .router-link {
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
        box-shadow: 0 0 4px 0 #000;
    }

    .header .router-link:active {
        box-shadow: none;
    }

    .header .router-link i {
        font-weight: light;
    }

    @media screen and ( max-aspect-ratio: 1/1 ) {
        .header .router-link {
            min-width: min(6vh, 8vw);
        }

        .header .router-link span {
            display: none;
        }
    }
</style>
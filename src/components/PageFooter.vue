<template>
    <div class="footer">
        <a href="https://cataas.com/cat/says/no%20email%20yet" class="mail">
            <i class="fa fa-envelope"></i>
        </a>
        <a href="https://cataas.com/cat/says/no%20tickets%20yet" class="tickets">
            Get Tickets
        </a>
        <a href="https://sexpression.org.uk" class="logo">
            <img src="@/assets/img/logo_nobg.png" alt="Sexpression Logo" draggable="false">
        </a>
    </div>
</template>

<style scoped>
    .footer {
        width: 100%;
        height: 10%;
        position: relative;
        white-space: nowrap;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
    }

    .footer a.mail {
        line-height: min(6vh, 8vw);
        font-size: min(3vh, 4vw);
        width: min(6vh, 8vw);
        position: absolute;
        left: 2vh;
        border-radius: 6vh;
        text-align: center;
        text-decoration: none;
        color: var(--colour-text-emphasis);
        background-color: var(--colour-emphasis);
    }

    .footer a.tickets {
        line-height: min(6vh, 8vw);
        font-size: min(3vh, 4vw);
        width: 50%;
        border-radius: 6vh;
        text-align: center;
        text-decoration: none;
        color: var(--colour-text-emphasis);
        background-color: var(--colour-emphasis);
    }

    .footer a.logo {
        position: absolute;
        right: 1vh;
        height: 100%;
        display: flex;
        align-items: center;
    }

    .footer a.logo img {
        max-height: 100%;
        max-width: 20vw;
    }
</style>

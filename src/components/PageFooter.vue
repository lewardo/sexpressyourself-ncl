<template>
    <div class="footer">
        <a href="https://eepurl.com/ix05Gs" class="mail">
            <i class="fa fa-envelope"></i>
        </a>
        <!-- <a href="#" class="tickets" @click.prevent="notickets"> -->
            <!-- {{ msg }} -->
        <!-- </a> -->
        <a href="https://www.eventbrite.co.uk/e/sexpression-national-conference-2023-tickets-729484697367" class="tickets">
           Get Tickets
        </a>
        <a href="https://sexpression.org.uk" class="logo">
            <img src="@/assets/img/logo_nobg.png" alt="Sexpression Logo" draggable="false">
        </a>
    </div>
</template>

<!-- <script>
    export default {
        data() {
            return {
                msg: `Get Tickets`,
            }
        },
        methods: {
            notickets() {
                this.msg = `Tickets live 02/10!`;
            }
        }
    }
</script> -->

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

    .footer a {
        color: var(--colour-text-emphasis);
        background-color: var(--colour-emphasis);
        box-shadow: 0 0 4px 0 #000;
    }

    .footer a:active {
        box-shadow: none;
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
    }

    .footer a.tickets {
        line-height: min(6vh, 8vw);
        font-size: min(3vh, 4vw);
        width: 50%;
        border-radius: 6vh;
        text-align: center;
        text-decoration: none;
    }

    .footer a.logo {
        position: absolute;
        right: 1vh;
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: flex-end;
        background-color: #00000000;
        border: none;
        box-shadow: none;
    }

    .footer a.logo img {
        max-height: 100%;
        max-width: 20vw;
    }
</style>

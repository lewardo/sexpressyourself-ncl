<script setup>
import PageTitle from '@/components/PageTitle.vue'
</script>

<template>
  <PageTitle title="Contact Us"/>
  
  <div class="contacts">
      <img src="@/assets/img/arrow.svg" class="arrow" alt="">
      <div class="mailing-list">
          Fill in the form on the left to join our mailing list for updates!
      </div>
      <div class="contact-mail">
          Or, contact us with any enquiries on <a href="mailto:newcastle@sexpression.org.uk">newcastle&#8203;@sexpression.org.uk</a>
      </div>
  </div>
</template>

<style scoped>
    @import '@/assets/view.css';


  .contacts {
        font-size: min(3vh, 6vw);
        width: 90%;
        flex-grow: 1;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        text-align: center;
        background-color: #00000020;
        border-radius: 24px;
        z-index: 2;
    }

    .contact-mail :is(a, a:visited) {
        color: #0f0a62;
    }

    .arrow {
        position: fixed;
        bottom: 10vh;
        left: -5vh;
        height: 40vh;
        transform: rotate(-60deg) scaleX(-1);
    }

    @media screen and ( max-aspect-ratio: 1/1 ) {
        .arrow {
            bottom: 10vh;
            left: -10vh;
            transform: rotate(-75deg) scaleX(-1);
        }
    }
</style>

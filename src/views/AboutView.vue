<script setup>
import PageTitle from '@/components/PageTitle.vue'
</script>

<template>
  <PageTitle title="About"/>

  <div class="content">
      <img src="@/assets/img/logo_full_nobg.png" alt="sexpression newcastle logo">
      <hr>
      <div class="info">
          Sexpression:&#8203;Newcastle is a thing
      </div>
  </div>
</template>

<style scoped>
    @import '@/assets/view.css';

  .content {
        width: 90%;
        display: flex;
        border-radius: 24px;
        overflow: hidden;
        background: #00000020;
    }

    .content hr {
        border: 1px solid #00000020;
    }

    @media screen and ( min-aspect-ratio: 4/5 ) {
        .content img {
            height: 100%;
        }

        .content .info {
            flex-grow: 1;
            padding: 24px;
        }
    }

    @media screen and ( max-aspect-ratio: 4/5 ) {
        .content {
            flex-direction: column;
            align-items: center;
        }

        .content img {
            height: 20vh;
        }

       .content .info {
            width: 100%;
            flex-grow: 1;
            padding: 0 4vh 2vh;
        }
    }
</style>

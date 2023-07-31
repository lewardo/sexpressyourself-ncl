<script setup>
import { RouterView } from 'vue-router'

import Header from '@/components/PageHeader.vue'
import Footer from '@/components/PageFooter.vue'
</script>

<template>
  <div class="app-background fullsize">
    <img src="@/assets/img/bg_ne.png" id="bg_ne" draggable="false">
    <img src="@/assets/img/bg_nw.png" id="bg_nw" draggable="false">
    <img src="@/assets/img/bg_se.png" id="bg_se" draggable="false">
    <img src="@/assets/img/bg_sw.png" id="bg_sw" draggable="false">
  </div>
  <div class="app-content fullsize">
    <Header />
    <RouterView />
    <Footer />
  </div>
</template>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Poppins&display=swap');
  @import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css');

  .app-background img {
    position: absolute;
  }

  #bg_ne {
      top: 0;
      right: 0;
      max-height: 20vmin;
  }

  #bg_nw {
      top: 0;
      left: 0;
      max-width: 25vmin;
  }

  #bg_se {
      top: 40%;
      right: 0;
      max-width: 20vmin;
  }

  #bg_sw {
      bottom: 0;
      left: 0;
      max-height: 20vmin;
  }

  .app-content {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    gap: 0;
  }
</style>

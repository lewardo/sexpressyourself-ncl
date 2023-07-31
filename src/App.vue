<script setup>
import { RouterView } from 'vue-router'

import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'
</script>

<template>
  <div class="app-background">
    <img src="@/assets/img/bg_ne.png" id="bg_ne" draggable="false">
    <img src="@/assets/img/bg_nw.png" id="bg_nw" draggable="false">
    <img src="@/assets/img/bg_se.png" id="bg_se" draggable="false">
    <img src="@/assets/img/bg_sw.png" id="bg_sw" draggable="false">
  </div>
  <div class="app-content">
    <Header></Header>
    <RouterView />
    <Footer></Footer>
  </div>
</template>

<style scoped>

</style>

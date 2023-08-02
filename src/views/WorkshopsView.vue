<script setup>
import PageTitle from '@/components/PageTitle.vue'

import CarouselWrapper from '@/components/CarouselWrapper.vue'
import CarouselSlide from '@/components/CarouselSlide.vue'
</script>

<template>
  <PageTitle title="Workshops" :schedule="true"/>

  <div class="content">
    <CarouselWrapper>
      <CarouselSlide name="one" prev="#three" next="#two">
        one
      </CarouselSlide>
      <CarouselSlide name="two" prev="#one" next="#three">
        two
      </CarouselSlide>
      <CarouselSlide name="three" prev="#two" next="#one">
        three
      </CarouselSlide>
    </CarouselWrapper>
  </div>
</template>

<style scoped>
  @import '@/assets/view.css';
  .content {
    width: 100%;
  }
</style>

<template>
  <div class="wrapper">
    <section class="home">
      <Navbar />
      <HomeContent />
    </section>
    <section class="sliderWrapper">
      <Slider />
    </section>
    <section class="videoArea">
      <Videos />
    </section>
    <section class="cardArea">
      <WhatThisEvent />
    </section>
    <section class="querstionsArea">
      <AskedQuestions />
    </section>
    <section class="footerArea">
      <Footer />
    </section>
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import HomeContent from '@/components/HomeContent.vue'
import Slider from '@/components/slider.vue'
import Videos from '@/components/Videos.vue'
import WhatThisEvent from '@/components/WhatThisEvent.vue'
import AskedQuestions from '@/components/AskedQuestions.vue'
import Footer from '@/components/Footer.vue'
export default {
    components:{
      Navbar,
      HomeContent,
      Slider,
      Videos,
      WhatThisEvent,
      AskedQuestions,
      Footer
    }
}
</script>

<style>
.wrapper{
  width: 100%;
  height: auto;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}
section{
  width: 100%;
  flex-direction: column;
  display: flex;
  flex-wrap: wrap;
}
.home{
  display: flex;
  flex-direction: column;
  gap: 80px;
  height: 100%;
  background:  url("../assets/img/header-background.png");
}
</style>
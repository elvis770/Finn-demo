
<template>
  <div class="home">
    <div class="nav">
      <Navbar/> 
    </div>
    <Hero/>
    <Slides/>
    <Timers/>
    <Section/>
    <Second/>
    <Activity/>

    <div class="foot">
      <Footer/>
    </div>
    
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Navbar from '@/components/Navbar.vue'
import Hero from '@/components/Hero.vue'
import Slides from '@/components/Slides.vue'
import Timers from '@/components/Timers.vue'
import Section from '@/components/Section.vue'
import Second from '@/components/Second.vue'
import Activity from '@/components/Activity.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'WorkView',
  components: {
    Navbar,
    Hero,
    Slides,
    Timers,
    Section,
    Second,
    Activity,
    Footer
  },
};
</script>

<style lang="scss">
*{
  margin-top: 14px;
    color: #fff;

    .foot{
      margin-bottom: 100px;
    }

}
</style>
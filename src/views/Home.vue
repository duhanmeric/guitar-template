<template>
  <div class="home">
    <app-campaign></app-campaign>
    <app-carousel></app-carousel>
    <app-desktop-info v-if="!MobileView"></app-desktop-info>
    <app-mobile-info v-else></app-mobile-info>
    <app-line class="home-line"></app-line>
  </div>
</template>

<script>
// @ is an alias to /src
import Campaign from '@/components/Common/Campaign.vue';
import Carousel from '@/components/Common/Carousel.vue';
import DesktopInfo from '@/components/Desktop/Information.vue';
import MobileInfo from '@/components/Mobile/Information.vue';
import Line from '@/components/Common/Line.vue';

export default {
  name: 'Home',
  components: {
    'app-campaign': Campaign,
    'app-carousel': Carousel,
    'app-desktop-info': DesktopInfo,
    'app-mobile-info': MobileInfo,
    'app-line': Line,
  },
  data(){
    return {
      MobileView: false,
    }
  },
  methods:{
    handleView(){
      this.MobileView = window.innerWidth <= 992;
    }
  },
  created(){
    this.handleView();
    window.addEventListener('resize',this.handleView);
    console.log("xd")
  },
}
</script>

<style>
.home-line{
  margin-top: 0px!important;
}
</style>

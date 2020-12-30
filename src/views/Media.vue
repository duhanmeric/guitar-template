<template>
  <div id="media">
    <app-desktop-media v-if="!MobileView"></app-desktop-media>
    <app-mobile-media v-else></app-mobile-media>
    <app-line class="media-line"></app-line>
  </div>
</template>

<script>
import DesktopMedia from '@/components/Desktop/MediaComp.vue';
import MobileMedia from '@/components/Mobile/MediaComp.vue';
import Line from '@/components/Common/Line.vue';

export default {
  name: "media",
  components: {
    'app-desktop-media': DesktopMedia,
    'app-mobile-media': MobileMedia,
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

<style scoped>
.media-line{
  margin: 10px 0!important;
}
</style>

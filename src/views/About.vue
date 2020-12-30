<template>
  <div class="about">
    <app-desktop-aboutcomp v-if="!MobileView"></app-desktop-aboutcomp>
    <app-mobile-aboutcomp v-else></app-mobile-aboutcomp>
    <app-desktop-line class="line"></app-desktop-line>
  </div>
</template>

<script>
import DesktopAboutComp from '@/components/Desktop/AboutComp.vue'
import MobileAboutComp from '@/components/Mobile/AboutComp.vue'
import desktopLine from '@/components/Common/Line.vue';
export default{
  components: {
    'app-desktop-aboutcomp': DesktopAboutComp,
    'app-mobile-aboutcomp': MobileAboutComp,
    'app-desktop-line': desktopLine,
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
};
</script>

<style scoped>
.line{
  margin: 0!important;
}
@media screen and (max-width:1024px) {
  .line{
    margin-bottom: 3rem!important;
  }
}
</style>

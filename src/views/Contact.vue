<template>
  <div id="contact">
    <app-desktop-contactComp v-if="!MobileView"></app-desktop-contactComp>
    <app-mobile-contactComp v-else></app-mobile-contactComp>
    <app-line></app-line>
  </div>
</template>

<script>
import DesktopContactComp from '@/components/Desktop/ContactComp.vue'
import MobileContactComp from '@/components/Mobile/ContactComp.vue'
import Line from '@/components/Common/Line.vue'

export default {
  name: "contact",
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
  components: {
    'app-desktop-contactComp': DesktopContactComp,
    'app-mobile-contactComp': MobileContactComp,
    'app-line': Line,
  },
}
</script>

<style scoped>
</style>

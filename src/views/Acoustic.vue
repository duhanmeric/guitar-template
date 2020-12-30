<template>
   <div id="acoustic">
     <app-desktop-acoustic v-if="!MobileView"></app-desktop-acoustic>
     <app-mobile-acoustic v-else></app-mobile-acoustic>
     <app-line-acoustic class="line"></app-line-acoustic>
   </div>
</template>

<script>
import DesktopAcoustic from '@/components/Desktop/AcousticComp.vue'
import MobileAcoustic from '@/components/Mobile/AcousticComp.vue'
import Line from '@/components/Common/Line.vue'
export default{
  components:{
    'app-desktop-acoustic': DesktopAcoustic,
    'app-mobile-acoustic': MobileAcoustic,
    'app-line-acoustic': Line,
  },
  data(){
    return {
      MobileView: false,
    }
  },
  methods:{
    handleView(){
      this.MobileView = window.innerWidth <= 1024;
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
#acoustic{
  padding: 0rem 0rem;
  background-color: white;
}

.line{
  margin-top: 1rem!important;
  margin-bottom: 1rem!important;
}

@media screen and (min-width:1024px){
  .line{
    margin-top: 1rem!important;
    margin-bottom: 0rem!important;
  }
}
</style>

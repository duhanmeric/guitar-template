<template>
   <div id="amplifiers">
     <app-desktop-amp v-if="!MobileView"></app-desktop-amp>
     <app-mobile-amp v-else></app-mobile-amp>
     <app-line-amp class="line"></app-line-amp>
   </div>
</template>

<script>
import DesktopAmp from '@/components/Desktop/AmpComp.vue'
import MobileAmp from '@/components/Mobile/AmpComp.vue'
import Line from '@/components/Common/Line.vue'
export default{
  components:{
    'app-desktop-amp': DesktopAmp,
    'app-mobile-amp': MobileAmp,
    'app-line-amp': Line,
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
#amplifiers{
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

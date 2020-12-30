<template>
   <div id="bass">
     <app-desktop-bass v-if="!MobileView"></app-desktop-bass>
     <app-mobile-bass v-else></app-mobile-bass>
     <app-line-bass class="line"></app-line-bass>
   </div>
</template>

<script>
import DesktopBass from '@/components/Desktop/BassComp.vue'
import MobileBass from '@/components/Mobile/BassComp.vue'
import Line from '@/components/Common/Line.vue'
export default{
  components:{
    'app-desktop-bass': DesktopBass,
    'app-mobile-bass': MobileBass,
    'app-line-bass': Line,
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
#bass{
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

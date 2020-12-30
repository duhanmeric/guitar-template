<template>
   <div id="electric">
     <app-desktop-electric v-if="!MobileView"></app-desktop-electric>
     <app-mobile-electric v-else></app-mobile-electric>
     <app-line-electric class="line"></app-line-electric>
   </div>
</template>

<script>
import DesktopElectric from '@/components/Desktop/ElectricComp.vue'
import MobileElectric from '@/components/Mobile/ElectricComp.vue'
import Line from '@/components/Common/Line.vue'
export default{
  components:{
    'app-desktop-electric': DesktopElectric,
    'app-mobile-electric': MobileElectric,
    'app-line-electric': Line,
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
#electric{
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

<template>
  <div id="app">
    <app-desktop-navbar v-if="!MobileView"></app-desktop-navbar>
    <app-mobile-navbar v-else @opened="emittedHeader"></app-mobile-navbar>
    <router-view class="rw" />
    <app-desktop-footer v-if="!MobileView"></app-desktop-footer>
    <app-mobile-footer v-else></app-mobile-footer>
  </div>
</template>

<script>
import DesktopNavbar from '@/components/Desktop/Master/Navbar.vue'
import MobileNavbar from '@/components/Mobile/Master/Navbar.vue'
import DesktopFooter from '@/components/Desktop/Master/Footer.vue'
import MobileFooter from '@/components/Mobile/Master/Footer.vue'

export default {
  data(){
    return {
      MobileView: false,
      isFlowing: true,
    }
  },
  methods:{
    handleView(){
      this.MobileView = window.innerWidth <= 992;
    },
    emittedHeader () {
      let dontFlow = document.querySelector("body");
      this.isFlowing = !this.isFlowing;
      console.log(this.isFlowing)
      if(this.isFlowing == false){
        dontFlow.classList.add("closeFlow");
      }
      else{
        dontFlow.classList.remove("closeFlow");
      }
    }
  },
  created(){
    this.handleView();
    window.addEventListener('resize',this.handleView);
    console.log("xd")
  },
  components: {
    'app-desktop-navbar': DesktopNavbar,
    'app-mobile-navbar': MobileNavbar,
    'app-desktop-footer': DesktopFooter,
    'app-mobile-footer': MobileFooter,
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600&display=swap');

:root{
  --first: #F44336; /* gitar kırmızısı */
  --second: #000; /* pure black */
  --second-ton: #111; /* daha açık siyah */
  --second-ton-second: #222; /* daha açık siyah */
  --third: #1b1b1b;  /* daha açık siyah */
  --fourth: #eee;  /* beyazımsı gri */
}
html,body{
  min-height: 100%;
  /* overflow: hidden!important; */
}

body.closeFlow{
  overflow: hidden!important;
}

#app {
  /* font-family: Avenir, Helvetica, Arial, sans-serif; */
  font-family: 'Open Sans', sans-serif;

  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.rw{
  margin-top: 60px;
}

@media screen and (max-width:1023px){
  .rw{
    margin-top: 60px;
  }
}
</style>

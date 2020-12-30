<template>
  <header id="mb-navbar" class="d-flex justify-content-between align-items-center">
    <div class="logo">
      <router-link to="/">
        <img src="@/assets/logo.png" class="w-100" alt="">
      </router-link>
    </div>
    <div class="cross" :class="{ degreed: isDegreed }" v-on:click="changeDegree">
      <div class="first"></div>
      <div class="second"></div>
    </div>
    <div id="nav" :class="{ degreed: isDegreed }">
      <div class="container d-flex flex-column justify-content-around">
        <router-link to="/electric-guitar">Electric Guitars</router-link>
        <router-link to="/bass-guitar">Bass Guitars</router-link>
        <router-link to="/acoustic-guitar">Acoustic Guitars</router-link>
        <router-link to="/amplifiers">Amplifies</router-link>
        <hr style="background-color: white;">
        <router-link to="/media">Media</router-link>
        <router-link to="/about">About</router-link>
        <router-link to="/contact">Contact</router-link>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  data(){
    return {
      isDegreed: false,
    }
  },
  methods: {
    changeDegree() {
      this.isDegreed = !this.isDegreed;
      this.$emit('opened');
    }
  }
}
</script>

<style scoped>
#mb-navbar{
  width: 100%;
  background-color: black;
  padding: .5rem 1rem;
  position: fixed;
  top: 0;
  z-index: 20;
}

.logo{
  width: 81px;
  height: 44px;
  transform: rotate(-10deg);
}

.logo img{
  width: 100%;
  height: 100%;
}

.cross{
  cursor: pointer;
  height: 10px;
  display: flex;
  justify-content: space-between;
  flex-direction: column;
}

.first,.second{
  width: 45px;
  height: 2px;
  background-color: white;
  transform-origin: 37% 50%;
  transition: transform .3s ease;
}

.cross.degreed .first{
  transform: rotate(45deg);
}

.cross.degreed .second{
  transform: rotate(-45deg);
}

#nav{
  width: 320px;
  min-height: 100vh;
  /* width: 100%; */
  position: absolute;
  border-top: 1px solid var(--first);
  top: 60px;
  right: -100%;
  background-color: black;
  padding: 1rem 0rem;
  transition: right 0.6s ease;
  text-align: left;
  text-transform: uppercase;
}

#nav a{
  font-size: 20px;
  color: white;
  text-decoration: none;
  position: relative;
  margin-top: .7rem;
  margin-bottom: 1rem;
}

#nav a::after{
  content: "";
  width: 0;
  height: 2px;
  background-color: var(--first);
  display: block;
  position: absolute;
  transition: width .5s ease;
}

#nav a:hover::after{
  width: 100%;
}

#nav.degreed{
  right: 0;
}
</style>

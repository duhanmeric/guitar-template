<template>
  <header id="navbar" class="d-flex justify-content-between align-items-center">
    <div class="logo">
      <router-link to="/">
        <img src="@/assets/logo.png" class="w-100" alt="">
      </router-link>
    </div>
    <div id="nav" class="d-flex justify-content-around align-items-center">
      <router-link to="/electric-guitar">Electric Guitars</router-link>
      <router-link to="/bass-guitar">Bass Guitars</router-link>
      <router-link to="/acoustic-guitar">Acoustic Guitars</router-link>
      <router-link to="/amplifiers">Amplifiers</router-link>
    </div>

    <div class="dots">
      <button class="btn drop-btn p-0 m-0 text-white">
        <i class="fas fa-chevron-down" style="font-size: 18px;"></i>
      </button>
      <div class="header-drop">
        <ul class="list-unstyled mb-0">
          <li>
            <router-link to="/media">Media</router-link>
          </li>
          <li>
            <router-link to="/about">About</router-link>
          </li>
          <li>
            <router-link to="/contact">Contact</router-link>
          </li>
        </ul>
      </div>
    </div>

  </header>
</template>


<style scoped>
header{
  background-color: var(--second-ton);
  padding: .5rem 2rem;
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 20;
  height: 60px;
}

.logo{
  width: 100px;
  height: 50px;
  transform: rotate(-10deg);
}

#nav {
  position: relative;
  top: 2px;
  width: 650px;
}

#nav a {
  color: white;
  text-decoration: none;
  font-size: 18px;
}

#nav a::after{
  content: "";
  width: 0;
  height: 2px;
  background-color: var(--first);
  display: block;
  transition: width .5s ease;
}

#nav a:hover::after{
  width: 100%;
}

.dots{
  position: relative;
  display: inline-block;
}

.header-drop{
  position: absolute;
  background-color: #111;
  min-width: 180px;
  z-index: 1;
  top: 18px;
  right: -100%;
  opacity: 0;
  text-align: left;
  visibility: hidden;
  transition: all .2s ease;
}

.dots:hover .header-drop {
  opacity: 1;
  visibility: visible;
  top: 100%;
}

.header-drop ul li a {
  color: white;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
}

.header-drop ul li a::after {
  content: "";
  width: 0;
  height: 2px;
  background-color: var(--first);
  display: block;
  transition: width .5s ease;
}

.header-drop ul li a:hover::after{
  width: 100%;
}

.header-drop a:hover {
  background-color: #555;
}

 @media screen and (min-width:992px) and (max-width:1440px){
  .logo{
    width: 90px;
    height: 45px;
  }
}

@media screen and (min-width:1440px){
  #nav a {
    font-size: 18px;
  }
}
</style>

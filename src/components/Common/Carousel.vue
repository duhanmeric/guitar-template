<template>
  <div id="guitar-carousel" class="carousel slide" data-bs-ride="carousel">
    <ol class="carousel-indicators">
      <li data-bs-target="#guitar-carousel" data-bs-slide-to="0" class="active"></li>
      <li data-bs-target="#guitar-carousel" data-bs-slide-to="1"></li>
      <li data-bs-target="#guitar-carousel" data-bs-slide-to="2"></li>
    </ol>
    <div class="carousel-inner h-100">
      <div class="carousel-item h-100 active">
        <img src="@/assets/landing/carousel1.jpg" class="d-block w-100 h-100" alt="...">
      </div>
      <div class="carousel-item h-100">
        <img src="@/assets/landing/carousel2.jpg" class="d-block w-100 h-100" alt="...">
      </div>
      <div class="carousel-item h-100">
        <img src="@/assets/landing/carousel3.jpg" class="d-block w-100 h-100" alt="...">
      </div>
    </div>
    <a class="carousel-control-prev" href="#guitar-carousel" role="button" data-bs-slide="prev">
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Previous</span>
    </a>
    <a class="carousel-control-next" href="#guitar-carousel" role="button" data-bs-slide="next">
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Next</span>
    </a>
</div>
</template>

<style>
#guitar-carousel{
  height: 520px;
  margin: 48px;
}

.carousel-item img{
  object-fit: cover;
}

@media screen and (max-width: 1023px){
  #guitar-carousel{
    height: 450px!important;
  }
}

@media screen and (min-width: 320px) and (max-width: 1024px){
  #guitar-carousel{
    margin: 0;
  }
}
</style>

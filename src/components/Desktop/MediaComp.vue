<template>
  <div id="ds-mediaComp">
    <div class="container w-100 py-5">
      <h1 class="media-title mb-5">GALLERY</h1>
      <div class="row d-flex align-items-center">
        <div class="col-md-4">
          <div class="row">
            <div class="media-photo smaller">
              <img src="@/assets/img/h3.jpg" class="w-100 h-100" alt="">
            </div>
          </div>
          <div class="row" style="margin-top: 40px;">
            <div class="media-photo smaller">
              <img src="@/assets/img/yedek4.jpg" class="w-100 h-100" alt="">
            </div>
          </div>
        </div>
        <div class="col-md-8">
          <div class="media-photo bigger">
            <img src="@/assets/img/yedek5.jpg" class="w-100 h-100" alt="">
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-md-4" style="margin-top: 40px;">
          <div class="media-photo smaller">
            <img src="@/assets/img/m1.jpg" class="w-100 h-100" alt="">
          </div>
        </div>
        <div class="col-md-4" style="margin-top: 40px;">
          <div class="media-photo smaller">
            <img src="@/assets/img/asdasd.jpg" class="w-100 h-100" alt="">
          </div>
        </div>
        <div class="col-md-4" style="margin-top: 40px;">
          <div class="media-photo smaller">
            <img src="@/assets/img/white.jpg" class="w-100 h-100" alt="">
          </div>
        </div>
      </div>
      <div class="row d-flex align-items-center">
        <div class="col-md-8">
          <div class="media-photo bigger" style="margin-top: 40px;">
            <img src="@/assets/img/h5.jpg" class="w-100 h-100" alt="">
          </div>
        </div>
        <div class="col-md-4">
          <div class="row">
            <div class="media-photo smaller" style="margin-top: 40px;">
              <img src="@/assets/img/h7.jpg" class="w-100 h-100" alt="">
            </div>
          </div>
          <div class="row" style="margin-top: 40px;">
            <div class="media-photo smaller">
              <img src="@/assets/img/learnn.jpg" class="w-100 h-100" alt="">
            </div>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-md-4" style="margin-top: 40px;">
          <div class="media-photo smaller">
            <img src="@/assets/img/m1.jpg" class="w-100 h-100" alt="">
          </div>
        </div>
        <div class="col-md-4" style="margin-top: 40px;">
          <div class="media-photo smaller">
            <img src="@/assets/img/asdasd.jpg" class="w-100 h-100" alt="">
          </div>
        </div>
        <div class="col-md-4" style="margin-top: 40px;">
          <div class="media-photo smaller">
            <img src="@/assets/img/white.jpg" class="w-100 h-100" alt="">
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "mediaComp",
}
</script>

<style scoped>
.media-title{
  font-size: 48px;
  font-weight: 600;
}

.bigger{
  height: 500px;
}

.smaller{
  height: 230px;
}

img{
  object-fit: cover;
}

.media-title{
  color: black;
  text-transform: uppercase;
  font-size: 48px;
}

@media screen and (min-width:1200px) {
  .container{
    width: 75%!important;
  }
}
</style>

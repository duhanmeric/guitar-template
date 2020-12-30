<template>
  <div id="mbAboutComp">
    <div class="row m-0">
      <div class="col-12 mx-auto p-0 first-col">
        <div class="about-photo p-0">
          <img src="@/assets/img/band2.jpg" alt="">
        </div>
      </div>
    </div>

    <div class="container">
      <div class="row m-0 my-5">
        <div class="col-lg-9 mx-auto about-col">
          <div class="title-container">
            <h1 class="about-title">
              ABOUT US
            </h1>
          </div>
          <div class="text-container">
            <p class="about-text">
              Our mission is what drives us to do everything possible to expand human potential. We do that by creating groundbreaking music innovations, by making our products more sustainably, by building a creative and diverse global team and by making a positive impact in communities where we live and work.
            </p>
          </div>
        </div>
      </div>
    </div>


    <section class="intro w-100 py-5">
      <div class="container section-container">
        <div class="row m-0">
          <div class="col-12">
            <div class="item-photo">
              <img src="@/assets/img/a1.jpg" alt="">
            </div>
          </div>
          <div class="col-12">
            <div class="item-description">
              <small class="small-description">INNOVATION</small>
              <h2 class="title-description mt-5 mb-3">
                WE DARE TO DESIGN THE FUTURE OF MUSIC
              </h2>
              <div class="info-description">
                <p>To make big leaps, we take big risks. Learn more about innovation team, platforms and partnerships.</p>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="container section-container middle-container">
        <div class="row m-0">
          <div class="col-12">
            <div class="item-photo">
              <img src="@/assets/img/a3.jpg" alt="">
            </div>
          </div>
          <div class="col-12">
            <div class="item-description">
              <small class="small-description">OUR TEAM</small>
              <h2 class="title-description mt-5 mb-3">
                A TEAM THAT'S EMPOWERED, DIVERSE AND INCLUSIVE
              </h2>
              <div class="info-description">
                <p>A love of music unites us. Learn more about Musical Company's global team.</p>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="container section-container">
        <div class="row m-0">
          <div class="col-12">
            <div class="item-photo">
              <img src="@/assets/img/a2.jpg" alt="">
            </div>
          </div>
          <div class="col-12">
            <div class="item-description">
              <small class="small-description">SUSTAINABLE BUSINESS INNOVATION</small>
              <h2 class="title-description mt-5 mb-3">
                PROTECTING THE FUTURE OF MUSIC
              </h2>
              <div class="info-description">
                <p>We believe in a fair, sustainable future one where everyone thrives on a healthy planet and level playing field. Learn how Musical Company is using the power of music to move the world forward.</p>
              </div>
            </div>
          </div>
        </div>
      </div>

    </section>

  </div>
</template>

<script>
export default {
  name: "",

}
</script>

<style scoped>
.first-col{
  width: 90%;
  margin: 30px;
}

.about-photo{
  height: 500px;
}

.about-photo img{
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.about-title{
  color: black;
  font-size: 46px;
  font-weight: 600;
  text-align: left;
}

.about-text{
  text-align: left;
  color: black;
  font-size: 18px;
}

.intro{
  background: #F7F7F7;
}

.item-photo{
  width: 100%;
  height: 250px;
}

.item-photo img{
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.item-description{
  text-align: left;
  color: black;
  margin: 24px 0;
}

.small-description{
  font-size: 16px;
}

.small-description::after{
  content: "";
  height: 2px;
  width: 50%;
  display: block;
  background: var(--first);
  margin: 3px 0;
}

.title-description{
  font-size: 24px;
  font-weight: 600;
}

.info-description{
  font-size: 16px;
}

.section-container{
  margin-top: 30px;
  margin-bottom: 30px;
}

.middle-container{
  margin-top: 120px;
  margin-bottom: 120px;
}

@media screen and (min-width:576px) {
  .item-photo{
    height: 400px;
  }
}
</style>

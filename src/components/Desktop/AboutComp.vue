<template>
  <div id="AboutComp">
    <div class="row mx-auto">
      <div class="col-11 mx-auto p-0">
        <div class="about-photo p-0">
          <img src="@/assets/img/band2.jpg" alt="">
        </div>
      </div>
    </div>
    <div class="row m-0 my-5">
      <div class="col-md-9 mx-auto">
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
    <section class="intro py-5">
      <div class="container section-container">
        <div class="row m-0">
          <div class="col-12 d-flex justify-content-around align-items-center">
            <div class="col-md-5">
              <div class="item-photo">
                <img src="@/assets/img/a1.jpg" alt="">
              </div>
            </div>
            <div class="col-md-6">
              <div class="item-description">
                <small class="small-description">INNOVATION</small>
                <!-- <hr class="w-50"> -->
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
      </div>

      <div class="container section-container middle-container">
        <div class="row m-0">
          <div class="col-12 d-flex justify-content-around align-items-center">
            <div class="col-md-6">
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
            <div class="col-md-5">
              <div class="item-photo">
                <img src="@/assets/img/a3.jpg" alt="">
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="container section-container">
        <div class="row m-0">
          <div class="col-12 d-flex justify-content-around align-items-center">
            <div class="col-md-5">
              <div class="item-photo">
                <img src="@/assets/img/a2.jpg" alt="">
              </div>
            </div>
            <div class="col-md-6">
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
      </div>

    </section>
  </div>
</template>

<script>
export default {
  name: "AboutComp",
}
</script>

<style scoped>
#AboutComp{
  width: 100%;
}

.col-11{
  width: 75%;
  margin: 48px;
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
  font-size: 60px;
  font-weight: 600;
  text-align: left;
}

.about-text{
  text-align: left;
  color: black;
  font-size: 20px;
}

.intro{
  background: #F7F7F7;
}

.item-photo{
  width: 100%;
  height: 600px;
}

.item-photo img{
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.item-description{
  text-align: left;
  color: black;
  margin-left: 20px;
}

.small-description{
  font-size: 18px;
}

.small-description::after{
  content: "";
  height: 2px;
  width: 50%;
  display: block;
  background: var(--first);
  margin: 5px 0;
}

.title-description{
  font-size: 28px;
  font-weight: 600;
}

.section-container{
  margin-top: 100px;
  margin-bottom: 100px;
}

.middle-container{
  margin-top: 150px;
  margin-bottom: 150px;
}

.info-description p{
  font-size: 18px;
}
</style>

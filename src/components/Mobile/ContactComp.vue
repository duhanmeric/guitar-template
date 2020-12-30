<template>
  <div id="mb-contactComp">
    <div class="container">
      <div class="main-row row m-0">
        <div class="col-12 motto-col pt-5 pb-2">
          <h1 class="motto-text">
            LIFE.
            <!-- <br> -->
            IT COULD BE
            <!-- <br> -->
            JUST THE THING
            <!-- <br> -->
            YOUR BRAND
            <!-- <br> -->
            NEEDS.
          </h1>
        </div>
        <div class="col-12 form-col">
          <form class="d-flex flex-column justify-content-between">
            <div class="form-element">
              <input type="text" class="w-100" id="contact-name" placeholder="Full Name">
            </div>
            <div class="form-element">
              <input type="email" class="w-100" id="contact-email" placeholder="Email">
            </div>
            <div class="form-element">
              <input type="text" class="w-100" id="contact-title" placeholder="Title">
            </div>
            <div class="form-element">
              <textarea name="contact-message" id="contact-message" class="w-100 contact-message" rows="7" placeholder="Message"></textarea>
            </div>
            <div class="btn-container w-100">
              <button type="submit" class="btn btn-outline-light w-50 submit-btn">SEND</button>
            </div>
          </form>
        </div>

        <div class="row m-0 noted-row">
          <div class="col-md-6 mx-auto">
            <div class="contact-photo">
              <img src="@/assets/contact/undraw.png" class="w-100" alt="">
            </div>
          </div>
        </div>

        <div class="row m-0">


          <div class="col-12 mx-auto p-0 office-col">
            <div class="office-card office-california px-3">
              <div class="office-info h-75">
                <h4 class="office-title">California Office</h4>
                <div class="hoverable-area">
                  <p class="office-text">4 N. Second Street Suite 800 San Jose, CA 95113</p>
                  <div class="office-contact">
                    <p class="office-phone">
                      <span class="phone-text">Phone: </span>+44 20 7234 3456
                    </p>
                    <p class="office-fax">
                      <span class="fax-text">Fax: </span>+44-208-1234567
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>

          <div class="col-12 p-0 office-col">
            <div class="office-card office-london px-3">
              <div class="office-info h-75">
                <h4 class="office-title">London Office</h4>
                <div class="hoverable-area">
                  <p class="office-text">221B Baker St, Marylebone, London NW1 6XE, UK</p>
                  <div class="office-contact">
                    <p class="office-phone">
                      <span class="phone-text">Phone: </span>+44 20 7234 3456
                    </p>
                    <p class="office-fax">
                      <span class="fax-text">Fax: </span>+44-208-1234567
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>

          <div class="col-12 p-0 office-col">
            <div class="office-card office-australia px-3">
              <div class="office-info h-75">
                <h4 class="office-title">Australia Office</h4>
                <div class="hoverable-area">
                  <p class="office-text">161 Sussex St, Sydney, NSW 2001</p>
                  <div class="office-contact">
                    <p class="office-phone">
                      <span class="phone-text">Phone: </span>+44 20 7234 3456
                    </p>
                    <p class="office-fax">
                      <span class="fax-text">Fax: </span>+44-208-1234567
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>

        </div>

      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "mb-contactComp",
}
</script>

<style scoped>
.motto-text{
  text-align: left;
  font-size: 40px;
  color: black;
  font-weight: 600;
}

.form-col{
  border-radius: 2rem;
  padding: 1rem 1rem;
}

form{
  height: 450px;
}

.form-element{
  border-bottom: 2px solid red;
}

input{
  height: 40px;
  border: none;
  outline: none;
  background: none;
}

.contact-message{
  resize: none;
  outline: none;
  border: none;
}

.btn-container{
  text-align: center;
}

.submit-btn{
  border-radius: 0;
  border: 2px solid #111;
  box-shadow: none;
  color: black;
}

.submit-btn:hover{
  background-color: #111;
  color: white;
}

.noted-row{
  margin-top: 100px!important;
  margin-bottom: 60px!important;
}

.office-col{
  /* margin: 40px 0; */
  margin-bottom: 50px;
}

.office-card{
  background-size: cover;
  height: 500px;
  transition: opacity .4s ease;
  position: relative;
}

.office-california{
  background-image: url('../../assets/contact/california.jpg');
}

.office-london{
  background-image: url('../../assets/contact/london.jpg');
}

.office-australia{
  background-image: url('../../assets/contact/australia.jpg');
}

.office-title{
  color: white;
  font-size: 32px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%,-50%);
  width: 100%;
  transition: all .5s ease;
}

.hoverable-area{
  position: absolute;
  top: 100%;
  left: 50%;
  width: 100%;
  transform: translate(-50%,-100%);
  transition: all .5s ease;
  opacity: 0;
  width: 90%;
}

.office-card:hover .office-title{
  top: 30%;
}

.office-card:hover .hoverable-area{
  top: 80%;
  opacity: 1;
}


.office-text{
  color: white;
  font-size: 20px;
}

.office-fax,.office-phone{
  color: white;
  font-size: 18px;
}


@media screen and (min-width:768px) {
  .form-col,.motto-col{
    width: 75%;
    margin: 0 auto;
  }
}

</style>

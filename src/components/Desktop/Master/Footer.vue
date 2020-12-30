<template>
  <footer id="ds-footer">
    <div class="footer-upper row mx-0 d-flex justify-content-around align-items-center w-75 mx-auto">
      <div class="col-3">
        <div class="follow-icons">
          <ul class="list-unstyled m-0 d-flex justify-content-around align-items-center">
            <li>
              <a href="#" class="media-link"><i class="fab fa-facebook-f"></i></a>
            </li>
            <li>
              <a href="#" class="media-link"><i class="fab fa-twitter"></i></a>
            </li>
            <li>
              <a href="#" class="media-link"><i class="fab fa-instagram"></i></a>
            </li>
            <li>
              <a href="#" class="media-link"><i class="fab fa-youtube"></i></a>
            </li>
          </ul>
        </div>
      </div>
      <div class="col-5">
        <div class="brand">BRAND</div>
      </div>
      <div class="col-3">
        <div class="description">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit.
        </div>
      </div>
    </div>
    <hr class="line w-75">
    <div class="footer-bottom row mx-0 d-flex justify-content-around align-items-center w-75 mx-auto">
      <div class="col-6">
        <div class="copyright">
          Copyright ©2020. All Rights Reserved.
        </div>
      </div>
      <div class="col-5 d-flex justify-content-around align-items-center">
        <div class="privacy">
          <router-link to="/privacy-policy">Privacy policy</router-link>
        </div>
        |
        <div class="terms-of-use">
          <router-link to="/terms-of-use">Terms of Use</router-link>
        </div>
        |
        <div class="cookie">
          <router-link to="/cookies">Cookie Policy</router-link>
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped>
#ds-footer{
  background-color: white;
  padding: 3rem 0;
}

.media-link i {
  font-size: 24px;
  color: black;
}

.brand{
  font-size: 32px;
  color: black;
  letter-spacing: 10px;
}

.description{
  color: black;
  text-align: left;
}

.line{
  width: 90%;
  margin: 50px auto;
  background-color: black;
}

.copyright{
  text-align: left;
  color: black;
}

.privacy a,.terms-of-use a,.cookie a{
  color: black;
  text-decoration: none;
}

.privacy a:hover,.terms-of-use a:hover,.cookie a:hover{
  color: #696969;
  text-decoration: underline;
}

@media screen and (min-width:992px) and (max-width:1440px){
  .footer-upper{
    width: 95%!important;
  }
  .footer-bottom{
    width: 95%!important;
    align-items: flex-start!important;
  }
  .line{
    width: 90%!important;
  }

}
</style>

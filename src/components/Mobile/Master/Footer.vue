<template>
  <footer id="mb-footer">
    <div class="row mx-0">
      <div class="brand">BRAND</div>
    </div>
    <div class="row fu-middle mx-0 mb-4 mt-2 mx-auto">
      <div class="description">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit.
      </div>
    </div>
    <div class="row mx-0">
      <div class="follow-icons">
        <ul class="list-unstyled m-0 d-flex justify-content-around align-items-center w-75 mx-auto">
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
    <div class="row mx-0 d-flex rules mt-4 w-75 mx-auto">
      <div class="privacy col-4">
        <router-link to="/privacy-policy">Privacy policy</router-link>
      </div>
      <div class="terms-of-use col-4">
        <router-link to="/terms-of-use">Terms of Use</router-link>
      </div>
      <div class="cookie col-4">
        <router-link to="/cookies">Cookie Policy</router-link>
      </div>
    </div>
    <div class="row mx-0 mt-4">
        <div class="copyright">
          Copyright ©2020. Musical Instruments Corporation. All Rights Reserved.
        </div>
    </div>
  </footer>
</template>

<style scoped>
#mb-footer{
  background-color: white;
  padding-top: 0rem;
  padding-bottom: 1rem;
}

.brand{
  font-size: 32px;
  letter-spacing: 10px;
  color: black;
}

.description{
  color: black;
}

.media-link i{
  font-size: 24px;
  color: black;
}

.fu-middle{
  width: 100%;
}

.privacy a,.terms-of-use a,.cookie a{
  color: black;
  text-decoration: none;
  font-size: 16px;
}


.privacy a:hover,.terms-of-use a:hover,.cookie a:hover{
  text-decoration: underline;
}

.copyright{
  color: black;
  font-size: 16px;
}

@media screen and (min-width:576px){
  .follow-icons{
    width: 60%;
    margin-right: auto!important;
    margin-left: auto!important;
  }

  .rules{
    width: 65%!important;
    margin-right: auto!important;
    margin-left: auto!important;
  }
}

@media screen and (min-width:768px){
  .rules{
    width: 60%!important;
    margin-right: auto!important;
    margin-left: auto!important;
  }
}
</style>

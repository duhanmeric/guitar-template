<template>
  <div class="mb-information pt-2">
    <div class="container">
      <div class="row mx-auto">
        <h1 class="hot-title mt-4">WHAT'S HOT?</h1>

        <div class="col-12 feature-col">
          <a href="#" class="feature-product">
            <div class="item-photo">
              <img src="@/assets/landing/learn.jpg" class="w-100" alt="">
            </div>
          </a>
          <a href="#" class="feature-product">
            <div class="item-title my-3">Item Title Goes Here</div>
          </a>
          <a href="#" class="feature-product">
            <span class="item-detail px-3 py-1">LEARN MORE</span>
          </a>
        </div>

        <div class="col-12 feature-col">
          <a href="#" class="feature-product">
            <div class="item-photo">
              <img src="@/assets/landing/lifestyle.jpg" class="w-100" alt="">
            </div>
          </a>
          <a href="#" class="feature-product">
            <div class="item-title my-3">Item Title Goes Here</div>
          </a>
          <a href="#" class="feature-product">
            <span class="item-detail px-3 py-1">LEARN MORE</span>
          </a>
        </div>

        <div class="col-12 feature-col">
          <a href="#" class="feature-product">
            <div class="item-photo">
              <img src="@/assets/landing/media.jpg" class="w-100" alt="">
            </div>
          </a>
          <a href="#" class="feature-product">
            <div class="item-title my-3">Item Title Goes Here</div>
          </a>
          <a href="#" class="feature-product">
            <span class="item-detail px-3 py-1">LEARN MORE</span>
          </a>
        </div>

        <div class="col-12 feature-col">
          <a href="#" class="feature-product">
            <div class="item-photo">
              <img src="@/assets/landing/choose.jpg" class="w-100" alt="">
            </div>
          </a>
          <a href="#" class="feature-product">
            <div class="item-title my-3">Item Title Goes Here</div>
          </a>
          <a href="#" class="feature-product">
            <span class="item-detail px-3 py-1">LEARN MORE</span>
          </a>
        </div>

      </div>
      <div class="row mx-auto quotes-row">
        <h1 class="quotes-title mt-3">THEY DON'T REGRET</h1>

        <div class="col-12 customer-col">
          <div class="customer-area d-flex flex-column justify-content-around">
            <div class="customer-header mt-3 d-flex justify-content-around align-items-center">
              <i class="fas fa-quote-left"></i>
              <div class="customer-name">Hinze Dam</div>
              <div class="customer-photo">
                <img src="@/assets/landing/customer2.jpg" class="w-100 h-100" alt="">
              </div>
            </div>
            <div class="customer-comment">
              <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eveniet reiciendis aut rerum rem officiis voluptatem consectetur, molestias eligendi cumque. Nesciunt, nulla. Nihil, architecto, quis! Pariatur.</p>
            </div>
          </div>
        </div>

        <div class="col-12 customer-col">
          <div class="customer-area d-flex flex-column justify-content-around">
            <div class="customer-header mt-3 d-flex justify-content-around align-items-center">
              <i class="fas fa-quote-left"></i>
              <div class="customer-name">Štefan Štefančík</div>
              <div class="customer-photo">
                <img src="@/assets/landing/customer1.jpg" class="w-100 h-100" alt="">
              </div>
            </div>
            <div class="customer-comment">
              <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eveniet reiciendis aut rerum rem officiis voluptatem consectetur, molestias eligendi cumque. Nesciunt, nulla. Nihil, architecto, quis! Pariatur.</p>
            </div>
          </div>
        </div>

        <div class="col-12 customer-col">
          <div class="customer-area d-flex flex-column justify-content-around">
            <div class="customer-header mt-3 d-flex justify-content-around align-items-center">
              <i class="fas fa-quote-left"></i>
              <div class="customer-name">Ayo Ogunseinde</div>
              <div class="customer-photo">
                <img src="@/assets/landing/customer3.jpg" class="w-100 h-100" alt="">
              </div>
            </div>
            <div class="customer-comment">
              <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eveniet reiciendis aut rerum rem officiis voluptatem consectetur, molestias eligendi cumque. Nesciunt, nulla. Nihil, architecto, quis! Pariatur.</p>
            </div>
          </div>
        </div>



      </div>
    </div>
  </div>
</template>

<script>
export default{
}
</script>

<style scoped>
.mb-information{
  background-color: white;
}

.hot-title{
  color: black;
  font-size: 38px;
  font-weight: 600;
}

.item-title{
  font-size: 18px;
}

.item-detail{
  font-size: 18px;
  font-weight: 600;
  border-bottom: 2px solid var(--first);
}

.feature-product{
  text-decoration: none;
  color: black;
}

.feature-col{
  margin: 30px 0;
}

.quotes-row{
  padding: 1.5rem 0;
}

.quotes-title{
  font-size: 38px;
  margin-top: 0px;
  color: black;
  font-weight: 600;
}

.customer-area{
  background-color: #111;
  text-align: left;
  height: 220px;
}

.customer-photo{
  width: 50px;
  height: 50px;
  border-radius: 50%;
}

.customer-photo img{
  object-fit: cover;
  border-radius: inherit;
}

.fa-quote-left{
  color: #eee;
  font-size: 24px;
}

.customer-name{
  color: white;
  font-size: 16px;
}

.customer-comment{
  width: 85%;
  margin: 0px auto 0px auto;
}

.customer-comment p{
  color: white;
  font-size: 14px;
}

.customer-col{
  margin: 20px 0;
}

@media screen and (min-width:375px) {
  .customer-area{
    height: 250px;
  }

  .customer-name{
    font-size: 18px;
  }

  .customer-comment p{
    font-size: 16px;
  }
}

@media screen and (min-width:425px) {
  .customer-area{
    height: 220px;
  }
}

@media screen and (min-width:768px) {
  .customer-area{
    height: 230px;
  }
}
</style>

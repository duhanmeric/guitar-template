<template>
  <div class="information mx-0">
    <div class="row mx-auto px-4">
      <h1 class="hot-title">WHAT'S HOT?</h1>

        <div class="col-3">
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

        <div class="col-3">
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

        <div class="col-3">
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

        <div class="col-3">
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
    <div class="row mx-auto px-4 justify-content-around quotes-row">
      <h1 class="quotes-title">THEY DON'T REGRET</h1>

      <div class="col-4 customer-col">
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

      <div class="col-4 customer-col">
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

      <div class="col-4 customer-col">
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
</template>

<script>
export default{
}
</script>

<style scoped>
.information{
  background-color: white;
  padding-bottom: 0rem;
  padding-top: 0rem;
}

.quotes-title{
  color: black;
}

.hot-title{
  margin-bottom: 36px;
  margin-top: 0;
  color: black;
  font-size: 48px;
  font-weight: 600;
}

.item-title{
  font-size: 18px;
}

.item-detail{
  font-size: 18px;
  font-weight: 500;
  border-bottom: 2px solid var(--first);
}

.feature-product{
  text-decoration: none;
  color: black;
}

.quotes-row{
  padding: 3rem 0 4rem 0;
}

.quotes-title{
  margin-top: 3rem;
  margin-bottom: 2rem;
  font-size: 48px;
  font-weight: 600;
}

.customer-area{
  background-color: #111;
  text-align: left;
  height: 260px;
}

.fa-quote-left{
  color: #eee;
  font-size: 24px;
}

.customer-name{
  color: white;
  font-size: 18px;
}

.customer-photo{
  width: 65px;
  height: 65px;
  border-radius: 50%;
}

.customer-photo img{
  object-fit: cover;
  border-radius: inherit;
}

.customer-comment{
  width: 85%;
  margin: 20px auto 20px auto;
}

.customer-comment p{
  color: white;
  margin-bottom: 0!important;
}

@media screen and (min-width:992px) and (max-width:1024px){
  .hot-title{
    margin-top: 36px;
    font-size: 42px;
  }

  .item-title{
    font-size: 16px;
  }

  .item-detail{
    font-size: 16px;
  }

  .quotes-title{
    font-size: 42px;
  }

  .customer-area{
    height: 300px;
  }
}

@media screen and (min-width:1024px) and (max-width:1440px){
  .hot-title{
    margin-top: 0px;
  }

  .quotes-row{
    padding-top: 2rem;
    padding-bottom: 4rem;
  }

  .customer-comment{
    width: 90%;
    margin: 0px auto 0px auto;
  }

  .customer-area{
    height: 250px;
  }

  .customer-comment p{
    color: white;
    margin-bottom: 1rem!important;
  }

}
</style>

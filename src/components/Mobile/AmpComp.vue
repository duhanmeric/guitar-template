<template>
  <div id="mb-amp">
    <div class="row mx-0">
      <h3 class="amp-title">Amplifiers</h3>

      <div class="top-control row mx-0 mx-auto d-flex justify-content-end align-items-center">
         <div class="col-2 w-auto p-0 nowidth d-flex align-items-center justify-content-end">
           <button class="btn sort-btn py-0 d-flex align-items-center justify-content-between">
             <span class="sort-text">SORT BY</span>
             <i class="fas fa-chevron-down"></i>
             <div class="drop">
               <ul class="list-unstyled mb-0">
                 <li>
                   <a href="#">Best Sellers</a>
                 </li>
                 <li>
                   <a href="#">Newest</a>
                 </li>
                 <li>
                   <a href="#">Lowest Price</a>
                 </li>
                 <li>
                   <a href="#">Highest Price</a>
                 </li>
               </ul>
             </div>
           </button>
         </div>
      </div>

      <div class="row mx-0 mt-0 products mx-auto d-flex justify-content-between align-items-center">
        <div class="col-12 p-0 prd-col my-4" v-for="prd in products" :key="prd.id">
          <div class="item-photo d-flex justify-content-center align-items-center">
            <!-- photo goes here -->
            photo goes here
          </div>
          <h5 class="product-title mt-1">
            {{ prd.title }}
          </h5>
        </div>
      </div>
    </div>
    <div class="row mx-0 justify-content-center align-items-center mt-3 mb-5">
      <ul class="pagination-list list-unstyled mb-0 w-auto d-flex justify-content-around align-items-center">
        <li class="pagination-item">
          <a href="#" class="pagination-link">
            <i class="fas fa-chevron-left"></i>
          </a>
        </li>
        <li class="pagination-item">
          <a href="#" class="pagination-link">1</a>
        </li>
        <li class="pagination-item">
          <a href="#" class="pagination-link">2</a>
        </li>
        <li class="pagination-item">
          <a href="#" class="pagination-link">3</a>
        </li>
        <li class="pagination-item">
          <a href="#" class="pagination-link">...</a>
        </li>
        <li class="pagination-item">
          <a href="#" class="pagination-link">9</a>
        </li>
        <li class="pagination-item">
          <a href="#" class="pagination-link">
            <i class="fas fa-chevron-right"></i>
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default{
  data(){
    return {
      dropped: false,
      products:[
        {
          id: 0,
          title:'title goes here',
        },
        {
          id: 1,
          title:'title goes here',
        },
        {
          id: 2,
          title:'title goes here',
        },
        {
          id: 3,
          title:'title goes here',
        },
        {
          id: 4,
          title:'title goes here',
        },
        {
          id: 5,
          title:'title goes here',
        },
        {
          id: 6,
          title:'title goes here',
        },
        {
          id: 7,
          title:'title goes here',
        },
        {
          id: 8,
          title:'title goes here',
        },
      ]
    }
  },
}
</script>

<style scoped>
.amp-title{
  margin-top: 2rem;
  margin-bottom: 1rem;
  color: black;
  font-size: 36px;
  font-weight: 600;
}

.prd-col{
  /* margin-top: 3rem;   */
}

.top-control{
  width: 90%;
}

.nowidth{
  position: relative;
}

.sort-btn{
  border-bottom: 2px solid var(--first);
  border-radius: 0;
  box-shadow: none;
}

.sort-text{
  font-size: 18px;
}

.fa-chevron-down{
  font-size: 18px;
  margin-left: 10px;
  transition: transform .3s ease;
  color: black;
}

.sort-btn:hover .fa-chevron-down{
  transform: rotate(180deg);
}

.drop{
 background-color: #222;
 position: absolute;
 top: 100%;
 left: 0;
 width: 100%;
 opacity: 0;
 visibility: hidden;
 transition: all .2s ease;
}

.sort-btn:hover .drop{
  visibility: visible;
  opacity: 1;
}

.drop ul li{
  width: 100%;
  text-align: left;
  transition: all .2s ease;
  display: flex;
}

.drop ul li:hover{
  background-color: #555;
}

.drop ul li a{
  color: white;
  text-decoration: none;
  display: block;
  padding: .4rem .5rem .4rem .5rem;
}

.products{
  width: 90%;
}

.col-12{
  cursor: pointer;
}

.item-photo{
  background-color: #ddd;
  height: 450px;
}

.item-photo{
  object-fit: cover;
}

.product-title{
  color: black;
  font-weight: 400;
}

.pagination-list{
  /* background: gray; */
  width: 90%!important;
  padding: 0!important;
}

.pagination-link{
  text-decoration: none;
  color: black;
  font-size: 20px;
}

.pagination-link:hover{
  text-decoration: underline;
}

@media screen and (min-width:425px){
  .products{
    width: 75%;
  }
  .top-control{
    width: 75%;
  }
  .col-12{
    width: 100%;
  }
  .pagination-list{
    width: 75%!important;
  }
}

@media screen and (min-width:576px){
  .products{
    width: 95%;
  }
  .top-control{
    width: 95%;
  }
  .col-12{
    width: 47%!important;
  }
  .pagination-list{
    width: 50%!important;
  }
}

@media screen and (min-width:768px){
  .products{
    width: 95%;
  }
  .col-12{
    width: 32%!important;
  }
  .pagination-list{
    width: 40%!important;
  }
}
</style>

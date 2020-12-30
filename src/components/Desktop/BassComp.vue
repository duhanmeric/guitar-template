<template>
   <div id="bass">
     <div class="row mx-0">
       <h3 class="bass-title mt-5">Bass Guitars</h3>

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

       <div class="row mx-0 products mx-auto d-flex justify-content-around align-items-center">
         <div class="col-4 product-square p-0 mt-4" v-for="prd in products" :key="prd.id">
           <div class="item-photo d-flex justify-content-center align-items-center">
             photo goes here
           </div>
           <h5 class="product-title mt-2">
             {{ prd.title }}
           </h5>
         </div>
       </div>
       <div class="row mx-0 justify-content-center align-items-center mt-5 my-4">
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
      ],
    }
  },
}
</script>

<style scoped>
.bass-title{
  color: black;
  font-size: 48px;
  margin-bottom: 0;
  font-weight: 600;
}

.top-control{
  width: 83.5%;
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
  font-size: 20px;
}

.fa-chevron-down{
  font-size: 18px;
  margin-left: 10px;
  color: black;
  transition: transform .3s ease;
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
  transition: opacity .2s ease;
}

.sort-btn:hover .drop{
  opacity: 1;
  visibility: visible;
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
  font-size: 16px;
  color: white;
  text-decoration: none;
  display: block;
  padding: .4rem .5rem .4rem .5rem;
}

.products{
  width: 90%;
}

.product-square{
  cursor: pointer;
  width: 26%;
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
  width: 23%!important;
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

@media screen and (min-width:1024px) and (max-width:1440px){
  .products{
    width: 95%;
  }
  .col-4{
    width: 28%;
  }
  .pagination-list{
    width: 25%!important;
  }
  .top-control{
    width: 90%;
  }
  .sort-area{
    width: 35%;
  }
}
</style>

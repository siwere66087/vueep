<template>

  <div class="testamonials" id="testamonials" >
          <div class="container" >
                <div class="card" style="width: 300px;height: 400px; margin: 10px;" v-for="item in testamonials" :key="item">
                  <div class="card-body">
                      <img :src="item.image"  class="card-img-top" >
                    <h5 class="card-title bold">{{ item.name }}</h5>  
                    <p>{{ item.description }}</p>   
                    <div class=" d-grid gap-2 col-6 mx-auto">
                    <a class="btn btn-dark" :href="item.facebook" target="_blank_">facebook</a>
                    <a  class="btn btn-dark" :href="item.github" target="_blank_">github</a>
                  </div>
                    </div>
                  </div>
               </div>
       </div>
  
  </template>
  
  
  <script>
  
  export default {
  data() {
     return {
     testamonials: [
    
   { name:'Nozipho mayila',
    description:"Siwe is a calm and open person and a great team player. ",
    image:'https://i.postimg.cc/j2C5G2GS/C11-Nozipho-Mayila-2.jpg'},
    {name:'Keren Bruce',
    description:'siwe  is a wonderful person to work with,she is a good listener as well.',
    image:'https://i.postimg.cc/6QLyZDrt/DSC-3514.jpg'},
   {name:'Asandile Langeni',
    description:'Siwe is a soft spoken person with great potential and ability to solve problems. she likes keeping to herself but is very caring',
    image:'https://i.postimg.cc/9Mc2RsXz/DSC-3626.jpg'},
   {name:'Gift Mahlangu',
   description:"She is a resilient person that strive for good thing not only for her but for others as well.",
   image:'https://i.postimg.cc/kM2jTMnZ/Gift-Mahlangu.jpg'},
   {name:'nontobeko Mhlongo',
   description:"She is a good person. she puts others before her and very understanding. shes great to work with.",
   image:'https://i.postimg.cc/DyzXgjd2/C11-Nontobeko-Mhlongo-2.jpg'}

    ] }
     }
    }
       
  
  
  
  
  </script>
  
  
  
  
  <style>
  
  
  .card-img-top{
    margin-top: 10px;
  }
  .container{
      display: grid; 
      grid-template-columns: 1fr 1fr 1fr;
      align-items: center  !important;;
      
    }
  #testamonials{
      padding-top: 125px;
     background-color: ghostwhite;
      
   
  }
   @media only screen and (max-width:970px) {
    .container{
      margin-top: 30px;
      display: grid; 
      grid-template-columns: 1fr 1fr;
      
    }
  }
  @media only screen and (max-width: 580px) {
    .container{
      display: grid; 
      grid-template-columns: 1fr;
      
    }
  }
  img{
    height: 12rem;
    object-fit: cover;
  }
  .btn::after {
    position: absolute;
    top: 25px;
    left: 0;
    content: "";
    width: 0%;
    height: 3px;
    background-color: rgba(255, 255, 255, 0.6);
    transition: all 0.5s;
  }
  
  .btn:hover::after {
    width: 100%;
  }
  
  
  
  
  /* RESPONSIVE */
  
  @media (max-width: 1600px) {
    .card {
      justify-content: center;
    }
  }
  
  </style>
  
  
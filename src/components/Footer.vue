<!-- <template>
   <div id="footer-container">
    <div id="footer">
      <div id="footer-contact">
        <p>{{ email }}</p>
        <p>{{ phone }}</p>
        <p>{{ socials }}</p>
      </div>
      <div id="footer-social">
       <div class="socials" ><a href=""><i class=" fab  fa-brands fa-facebook fa-2xl" ></i></a> </div>
        <div class="socials"> <a href=""><i class=" fab  fa-brands fa-twitter fa-2xl"></i></a></div>
        <div class="socials"><a href=""><i class=" fab  fa-brands fa-linkedin fa-2xl"></i></a></div>
        <div class="socials"><a href=""><i class=" fab  fa-brands fa-github fa-2xl"></i></a></div>
      </div>
    </div>
    <div id="copyright">
      <p>&copy;{{copyright }}</p>
    </div>
   </div>
</template>

<script>
    export default {
      data() {
        return {
            email:'sivuyisiwe.mgijima6@gmail.com',
            phone: '0683150682',
            copyright: 'copyright reserved developed by s.mgijima 2023'
        }
      },  
    }
</script>

<style scoped>


#footer-container{
  padding-top:20px;
  margin-top:20px;
  width:100vw;
  color:white;
  background-color:#1a1a1a;
  display:flex;
  flex-direction:column;
  align-items:center;
}
#footer{
  display:flex;
  justify-content:space-around;
  align-items:center;
  width:100%;
}
#footer-contact{
  text-align:right;
}
#footer-social{
  width:20%;
  display : flex;
  justify-content : space-between;
}
.socials a i {

width: 50px;
height: 50px;
border-radius: 50%;
/* background-color: #fff; */

}


#footer-social div i{
  height:50px ;
  width:50px;
  padding-top: 15px;

  border-radius:50%;
}
#address p {
  font-size:0.5em;
}




#copyright{
    margin-right: 45rem;
}
</style> -->





<template>
  <div class="footer">
      <footer>
<div class="row primary">
<div class="column socials">


<div class="social">
  <a href=""><a href=""><i class=" fab  fa-brands fa-facebook " ></i></a></a>
  <a href=""><a href=""><i class=" fab  fa-brands fa-twitter" ></i></a></a>
  <a href=""><a href=""><i class=" fab  fa-brands fa-twitter" ></i></a></a>
</div>

<div class="column subscribe">
<h3>contact me @</h3>
<i class="fa fa-envelope"> Email me at siwecele@gmail.com</i>


</div>

</div>

<div class="row copyright">
 <p>Copyright  reserved&copy; made by s.mgijima 2023 </p>
</div>
</div>
</footer>

  </div>
</template>

<script>
  export default {
      
  }
</script>

<style  scoped>
footer {
height: 10px;
color: #eaecf6;
font-size: 16px;
height: 30px;
padding-top:40px !important ;
}

.row {
padding: 1em 1em;
}
.row.primary {
display: grid;
grid-template-columns: 2fr 1fr ;
align-items: stretch;
}
.column {
width: 100%;
display: flex;
flex-direction: column;
padding: 0 2em;
min-height: 15em;
}
h3 {
width: 100%;
text-align: left;
color: #000000;
font-size: 1.4em;
padding: 10px;
white-space: nowrap;
}
/*  */
div.social {
display: flex;
justify-content: space-around;
font-size: 2.4em;
flex-direction: row;
margin-top: 0.5em;
}
.social i {
color: #e6e7e9;
}
.social i:hover{
  color:#ed822a
}

.copyright {
padding: 0.3em 1em;
background-color: rgba(15, 7, 7, 0);
}
.footer-menu{
float: left;
margin-top: 10px;


}

.footer-menu a{
color: #727476  ;
padding: 6px;
text-decoration: none;
}
.footer-menu a:hover{
color: black;
}
.copyright p {
font-size: 0.9em;
text-align: right;
}
@media screen and (max-width: 850px) {
.row.primary {
  grid-template-columns: 1fr;
}

}

</style>
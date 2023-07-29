<template>
    <footer class="footer">
     <div class="container">
       <div class="row">
         <div class="footer-col">
           <h4>About Teknotes.id</h4>
           <ul>
             <li><a href="#">About us</a></li>
             <li><a href="#">Contact us</a></li>
             <li><a href="#">Blog</a></li>
             <li><a href="#">Our service</a></li>
             <li><a href="#">Carrers</a></li>
           </ul>
         </div>
         <div class="footer-col">
           <h4>Product</h4>
           <ul>
             <li><a href="#">Flights</a></li>
             <li><a href="#">Trains</a></li>
             <li><a href="#">Hotels</a></li>
             <li><a href="#">Flights + Hotel</a></li>
             <li><a href="#">Eats</a></li>
             <li><a href="#">Paylater</a></li>
             <li><a href="#">Xperience</a></li>
           </ul>
         </div>
         <div class="footer-col">
           <h4>Guide and Help</h4>
           <ul>
             <li><a href="#">Care</a></li>
             <li><a href="#">Privacy Policy</a></li>
             <li><a href="#">Terms and Condition</a></li>
             <li><a href="#">Mitra</a></li>
           </ul>
         </div>
         <div class="footer-col">
           <h4>Follow us on</h4>
           <div class="social-media">
             <a href="https://www.instagram.com/p/CvPmMSYP2Vv/">
                <img src="https://img.freepik.com/free-vector/instagram-vector-social-media-icon-7-june-2021-bangkok-thailand_53876-136728.jpg?w=740&t=st=1690601563~exp=1690602163~hmac=fbe429b4504a0d4a7f4f4ed440b68d66814d8111c1fa0561ea896d4786363ca3" alt=""><i class="fab fa-instagram"></i></a>
           </div>
         </div>
       </div>
     </div>
   </footer>
   <div class="fixed-footer">
     <div class="container">Copyright &copy; 2023 SmkAssalaam & vinntzy</div>
   </div>
  </template>
  
  <style>
  body {
  line-height: 1.5;
  font-family: "Poppins", sans-serif;
  }
  * {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  }
  .container {
  max-width: 1170px;
  margin: auto;
  }
  .row {
  display: flex;
  flex-wrap: wrap;
  }
  ul {
  list-style: none;
  }
  .footer {
   background: linear-gradient(
       120deg,
       #1c99fe 20.69%,
       #7644ff 50.19%,
       #1900FF 79.69%
   );
  padding: 70px 0;
  }
  .footer-col {
  width: 25%;
  padding: 0 15px;
  }
  .footer-col h4 {
  font-size: 18px;
  color: rgba(255, 255, 255, 1);
  text-transform: capitalize;
  margin-bottom: 35px;
  font-weight: 500;
  position: relative;
  }
  .footer-col h4::before {
  content: "";
  position: absolute;
  left: 0;
  bottom: -10px;
  background-color: rgba(0, 3, 255, 0.8);
  height: 2px;
  box-sizing: border-box;
  width: 50px;
  }
  .footer-col ul li:not(:last-child) {
  margin-bottom: 10px;
  }
  .footer-col ul li a {
  font-size: 16px;
  text-transform: capitalize;
  color: rgba(255, 255, 255, 1);
  text-decoration: none;
  font-weight: 300;
  color: #bbbbbb;
  display: block;
  transition: all 0.3s ease;
  }
  .footer-col ul li a:hover {
  color: rgba(0, 3, 255, 0.8);
  padding-left: 8px;
  }
  .footer-col .social-media a {
  display: inline-block;
  height: 40px;
  width: 40px;
  background-color: rgba(255, 255, 255, 0.2);
  margin: 0 10px 10px 0;
  text-align: center;
  line-height: 40px;
  border-radius: 50%;
  color: rgba(255, 255, 255, 0.5);
  margin: 0 10px 10px 0;
  transition: all 0.5s ease;
  }
  .footer-col .social-media a:hover {
  color: rgba(0, 3, 255, 0.8);
  background-color: rgba(236, 236, 236, 0.8);
  }
  .fixed-footer {
   width: 100%;
   position: relative;
   background: #4000FF;
   margin: 0 10px 10px 0;
   padding: 10px 0;
   color: rgba(255, 255, 255, 1);
   text-align: center;
  }
  .fixed-footer {
   bottom: 0;
  }
  
  @media (max-width: 767px) {
  .footer-col {
   width: 50%;
   margin-bottom: 30px;
  }
  }
  @media (max-width: 574px) {
  .footer-col {
   width: 100%;
  }
  }
  </style>
# FormDesign
Design of Form 
html:
<!DOCTYPE html>   
  <html lang="en">   
  <head>   
   <meta charset="UTF-8" />   
   <meta http-equiv="X-UA-Compatible" content="IE=edge" />   
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />   
   <title> Flex Hover Slider</title>   
   <link rel="stylesheet" href="menuncrm.css">  
  </head>   
  <body>   
   <div class="flex-container">  
     <div class="spinner"><p>  
       <div class="cube1"></div>  
       <div class="cube2"></div>  
       Loading...  
       </p>  
     </div>  
	 
<?php
                                    /*CRM System*/
                     /* Developed by Oswaldo Jesús Marín Pagés*/
                    /*Enlaces de la diferentes areas del CRM*/

?>

     <div class="flex-slide home">  
       <div class="flex-title flex-title-home">Centros</div>  
       <div class="flex-about flex-about-home"><p>Click here to navigate to the home section of the Centros</p></div>  
     </div>  
     <div class="flex-slide home">  
       <div class="flex-title flex-title-home">Formacion</div>  
       <div class="flex-about flex-about-home"><p>Click here to navigate to the home section of the Formacion</p></div>  
     </div>  
     <div class="flex-slide home">  
       <div class="flex-title flex-title-home">Bolsa de Empleo</div>  
       <div class="flex-about flex-about-home"><p>Click here to navigate to the home section of the Bolsa de Empleo</p></div>  
     </div>  
     <div class="flex-slide home">  
       <div class="flex-title flex-title-home">Tecnologia</div>  
       <div class="flex-about flex-about-home"><p>Click here to navigate to the home section of the Tecnologia</p></div>  
     </div>
     
   <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>  
   <script src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/769286/jquery.waitforimages.min.js"></script>
   <script src="menu11.js"></script>  
  </body>   
  </html>   

  css:
  @import url('https://fonts.googleapis.com/css?family=Raleway');  
$defaultSeconds: 3s;
body {  
      margin: 0;  
      padding: 0;  
      font-family: 'Robato', sans-serif;  
 }  
 
 .flex-container {  
      position: absolute;  
      height: 100vh;  
      width: 100%;  
      display: -webkit-flex; /* Safari */  
      display: flex;  
      overflow: hidden;  
      @media screen and (max-width: 768px) {  
           flex-direction: column;  
      }  
 }  
 
  .flex-title {  
      color: #f1f1f1;  
      position: relative;  
      font-size: 6vw;  
      margin: auto;  
      text-align: center;  
      transform: rotate(90deg);  
      top: 15%;  
      -webkit-transition: all 500ms ease;  
      -moz-transition: all 500ms ease;  
      -ms-transition: all 500ms ease;  
      -o-transition: all 500ms ease;  
      transition: all 500ms ease;  
      @media screen and (max-width: 768px) {  
           transform: rotate(0deg) !important;  
      }  
 }  

 .flex-about {  
      opacity: 0;  
      color: #ffffff;  
      position: relative;  
      width: 70%;  
      font-size: 2vw;  
      padding: 5%;  
      top: 20%;  
      border: 2px solid #f1f1f1;  
      border-radius: 10px;  
      line-height: 1.3;  
      margin: auto;  
      text-align: left;  
      transform: rotate(0deg);  
      -webkit-transition: all 500ms ease;  
      -moz-transition: all 500ms ease;  
      -ms-transition: all 500ms ease;  
      -o-transition: all 500ms ease;  
      transition: all 500ms ease;  
      @media screen and (max-width: 768px) {  
           padding: 0%;  
           border: 0px solid #f1f1f1;  
      }  
 } 

.flex-slide {  
      -webkit-flex: 1; /* Safari 6.1+ */  
      -ms-flex: 1; /* IE 10 */    
      flex: 1;  
      cursor: pointer;  
      -webkit-transition: all 500ms ease;  
      -moz-transition: all 500ms ease;  
      -ms-transition: all 500ms ease;  
      -o-transition: all 500ms ease;  
      transition: all 500ms ease;  
      @media screen and (max-width: 768px) {  
           overflow: auto;  
           overflow-x: hidden;  
      }  
 }  

.flex-slide p {  
      @media screen and (max-width: 768px) {  
           font-size: 2em;  
      }  
 }  

 .flex-slide ul li {  
      @media screen and (max-width: 768px) {  
           font-size: 2em;  
      }  
 }   
 .flex-slide:hover {  
      -webkit-flex-grow: 3;  
      flex-grow: 3;  
 }  

.home {  
      height: 100vh;  
      background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url(img/laptop.jpg);  
      background-size: cover;  
      background-position: center center;  
      background-attachment: fixed;  
      @media screen and (min-width: 768px) {  
           animation: aboutFlexSlide $defaultSeconds 1;  
           animation-delay: 0s;  
      }  
 }   

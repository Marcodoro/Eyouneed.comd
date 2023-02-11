<template>
  <div class="all">
    <div class="page">
       <menu>
         <div class="hamburger">
              <img src="https://cdn-icons-png.flaticon.com/512/8860/8860952.png" height="28px" />
         </div>
        <div class="login">
           Login
        </div>
        <div class="menu">
          Home
        </div>
        <div class="about">
         About
        </div>
       </menu>
    </div>
    <div class="rest">
       <div class="getstarted">
          <div class="learncode">
             <div class="text-code">Learn Web dev</div>
             <br>
               <button class="button-85" role="button"><span class="btn-text">Now and Free</span></button>
          </div>
       </div>
       <div class="line"></div>
    </div>
    
  </div> 
 </template>
 
 <script>
 
 export default {
   name: 'App',
   components: {
   },
   data() {
     return {
       see: "scoped",
     }
   }
 }
 </script>
 
 <style>
 .line {
   width: 100%;
   height: 2vw;
   bottom: 30vh;
   position: absolute;
   background-color: transparent;
   box-shadow: rgba(0, 0, 0, 0.4) 0px 2px 4px, rgba(0, 0, 0, 0.3) 0px 7px 13px -3px, rgba(0, 0, 0, 0.2) 0px -3px 0px inset;
 }
 .getstarted {
   display: flex;
   justify-content: center;
   width: 50%;
   height: 45vh;
   box-shadow: rgba(0, 0, 0, 0.19) 0px 10px 20px, rgba(0, 0, 0, 0.23) 0px 6px 6px;
   background-color: rgba(255, 0, 0, 0);
 }
 .learncode {
   display: flex;
   justify-content: center;
   flex-direction: column;
 }
 .text-code {
   font-size: 5.8vw;
   font-weight: bolder;
   background: #00FF00;
 background: linear-gradient(to left, #00FF00 0%, #00FFFF 100%);
 -webkit-background-clip: text;
 -webkit-text-fill-color: transparent;
   font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
 }
 .rest {
   display: flex;
   flex-direction: row;
   justify-content: center;
   align-items: center;
   margin: 50px 0px;
 }
 .hamburger {
   justify-content: left;
   margin: 10px -10%;
 }
 menu {
   display: flex;
   justify-content: space-between;
   align-items: center;
   overflow: hidden;
   box-shadow: rgba(0, 0, 0, 0.3) 0px 19px 38px, rgba(0, 0, 0, 0.22) 0px 15px 12px;
   margin: -5px 0px;
   height: 4vh;
   min-height: 30px;
 }
 .login {
   font-size: 3.9vw;
   background: #2770CF;
   background: linear-gradient(to right, #2887a4 49%, #11c1d4 100%);
   -webkit-background-clip: text;
   -webkit-text-fill-color: transparent;
   font-weight: bolder;
   font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
 }
 .about {
   font-size: 3.9vw;
   background: #2770CF;
   background: linear-gradient(to right, #2770CF 49%, #40C1CF 100%);
   -webkit-background-clip: text;
   -webkit-text-fill-color: transparent;
   font-weight: bolder;
   font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
 }
 .about:hover {
   text-decoration: underline;
 }
 .home:hover {
   text-decoration: underline;
 }
 .login:hover {
   text-decoration: underline;
 }
 .menu {
   font-size: 3.9vw;
   background: #2770CF;
   background: linear-gradient(to right, #2770CF 49%, #40C1CF 100%);
   -webkit-background-clip: text;
   -webkit-text-fill-color: transparent;
   font-weight: bolder;
   font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
 }
 body {
   height: 1000px;
   overflow-x: hidden;
   background: rgb(70,140,166);
   background: linear-gradient(90deg, rgb(38, 90, 108) 0%, rgb(10, 53, 62) 30%, rgba(2,0,36,1) 96%);
 }
 @media only screen and (max-width: 412px) {
   .about {
     font-size: 4.9vw;
   }
   .menu {
     font-size: 4.9vw;
   }
   .login {
     font-size: 4.9vw;
   }
   .getstarted {
     max-height: 150px;
   }
   .line {
     bottom: 55vh;
   }
 }
 @media only screen and (min-width: 1200px) {
   .about {
     font-size: max(30px);
   }
   .menu {
     font-size: max(30px);
   }
   .login {
     font-size: max(30px);
   }
 }
 @media only screen and (min-width: 900px) {
  .about {
     font-size: max(35px);
   }
  .menu {
     font-size: max(35px);
   }
  .login {
     font-size: max(35px);
   }
   menu {
     min-height: 50px;
   }
 }
 @media only screen and (min-width: 1880px) {
   menu {
     min-height: 60px;
   }
 }
 :root {
   height: 1000px;
   overflow-x: hidden;
   background: rgb(70,140,166);
   background: linear-gradient(90deg, rgb(38, 90, 108) 0%, rgb(10, 53, 62) 30%, rgba(2,0,36,1) 96%);
 }
 html {
    height: 100%;
   overflow: auto;
   background: rgb(70,140,166);
   background: linear-gradient(90deg, rgb(38, 90, 108) 0%, rgb(10, 53, 62) 30%, rgba(2,0,36,1) 96%);
 }
 html {
   overflow: hidden;
   height: 100%;
 }
 
 
 /* Button styles */
 /* CSS */
 .button-85 {
   border: none;
   outline: none;
   color: rgb(255, 255, 255);
   background: #111;
   cursor: pointer;
   position: relative;
   z-index: 0;
   border-radius: 4px;
   height: 12vw;
   max-height: 160px;
   max-width: 470px;
   width: 40vw;
   user-select: none;
   -webkit-user-select: none;
   touch-action: manipulation;
   font-weight: bolder;
 }
 
 .button-85:before {
   content: "";
   background: linear-gradient(
     45deg,
     #ff0000,
     #ff7300,
     #fffb00,
     #48ff00,
     #00ffd5,
     #002bff,
     #7a00ff,
     #ff00c8,
     #ff0000
     );
   position: absolute;
   top: -2px;
   left: -2px;
   background-size: 400%;
   z-index: -1;
   filter: blur(5px);
   -webkit-filter: blur(5px);
   width: calc(100% + 4px);
   height: calc(100% + 4px);
   animation: glowing-button-85 20s linear infinite;
   transition: opacity 0.3s ease-in-out;
   border-radius: 4px;
 }
 
 @keyframes glowing-button-85 {
   0% {
     background-position: 0 0;
   }
   50% {
     background-position: 400% 0;
   }
   100% {
     background-position: 0 0;
   }
 }
 
 .button-85:after {
   z-index: -1;
   content: "";
   position: absolute;
   width: 100%;
   height: 100%;
   background: #222;
   left: 0;
   top: 0;
   border-radius: 4px;
 }
 .btn-text {
   font-size: 4.5vw;
 } 
 @media only screen and (min-width: 900px) {
    .btn-text {
   font-size: max(50px);
    }
    .text-code {
     font-size: max(60px);
    }
 }
 @media only screen and (min-width: 1000px) {
    .btn-text {
   font-size: max(65px);
    }
    .text-code {
     font-size: max(56px);
    }
    menu {
     min-height: 50px;
    }
    .line {
     bottom: 27%;
    }
 }
 @media only screen and (min-width: 1100px) {
    .btn-text {
   font-size: max(52px);
    }
    .text-code {
     font-size: max(65px);
    }
 }
 </style>
 
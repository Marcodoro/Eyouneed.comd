 
<script>
 
 export default {
   name: 'App',
   components: {

  },
   data() {
     return {
       open: false,
      }
  },
  methods: {
    open() {

    }
  },
}
  </script>
<template>
  <div class="all">
    <div class="page">
       <menu>
         <div class="hamburger" @click="open == true">
              <span class="line1"></span>
              <span class="line2"></span>
              <span class="line3"></span>
              <span class="line4"></span>
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
    <div class="open" v-if="open == true">
      
    </div>
    <div class="rest">
       <div class="getstarted">
          <div class="learncode">
             <div class="text-code">Learn Web dev</div>
             <br>
               <button class="button-85" role="button"><span class="btn-text">Now and Free</span></button>
          </div>
       </div>
      </div>
       <div class="line"></div>
       <br>
          <div class="courses">
            <div class="border">
              <div class="fix">
                <div class="courses-text">
                  Courses that we offer &nbsp; 
                </div>
                <a href="" class="see-all">See all </a>
              </div>
              <br>
              <div class="scroll">
                <img src="https://via.placeholder.com/150/0000FF/808080 ?Text=PAKAINFO.com" alt="" height="250px">
                <img src="https://via.placeholder.com/150/0000FF/808080 ?Text=PAKAINFO.com" alt="" height="250px">
                <img src="https://via.placeholder.com/150/0000FF/808080 ?Text=PAKAINFO.com" alt="" height="250px">
                <img src="https://via.placeholder.com/150/0000FF/808080 ?Text=PAKAINFO.com" alt="" height="250px">
                <img src="https://via.placeholder.com/150/0000FF/808080 ?Text=PAKAINFO.com" alt="" height="250px">
              </div>
            </div>
      </div>  
      <footer>
        <div class="down">
          <div class="icons">
             
          </div>
          <div class="icons">
             
          </div>
          <div class="icons">
             
           </div>
        </div>
      </footer>     
  </div> 
</template>

 <style>
footer {
  position: fixed;
  margin: 90% 0px;
  width: 100vw;
  height: 40px;
  background-color: red;
}
.down {
  position: fixed;
  margin: 0% 0px;
  width: 100vw;
  height: 40px;
  background-color: red;
}
 .scroll {
  width: 60vw;
  display: flex;
  flex-direction: row;
  overflow-x: scroll;
 }
 .fix {
  display: flex;
  gap: 10px
 }
 .see-all {
  color: rgb(39, 150, 107);
 }
.courses {
  display: flex;
  justify-content: center;
  width: 100vw;
  font-weight: bolder;
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}
.border { 
  border: 4px solid;  border-image-slice: 1;  border-width: 3px;
  height: 50vh;
  border-radius: 4px;
  border-image-source: linear-gradient(to left, #743ad5, #19806f);
}
.courses-text {
  background: #8442CF;
  background: linear-gradient(to right, #8442CF 0%, #3C36FF 32%, #C53ACF 83%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  margin: 0 10px;
}

body::-webkit-scrollbar-x {
  display: none;
}
body::-webkit-scrollbar{
  display: none;
}
 .open {
  height: 100%;
  width: 20%;
  background-color: #111;
 }
 .hamburger {
  display: flex;
  justify-content: center;
  flex-direction: column;
  gap: 0.2vw;
 }
 .line1 {
  max-height: 7px;
  max-width: 74px;
  width: 7vw;
  border-radius: 40px;
  height: 1vw;
  background-color: #00FFFF;background: rgb(10, 47, 69);
background: linear-gradient(90deg, rgb(0, 24, 36) 3%, rgba(18,88,102,1) 73%, rgba(70,140,166,1) 100%);
 }
 .line2 {
  max-height: 7px;
  max-width: 54px;
  width: 4.5vw;
  border-radius: 40px;
  height: 1vw;background: rgb(2,0,36);
background: linear-gradient(90deg, rgb(0, 32, 36) 3%, rgba(18,88,102,1) 73%, rgba(70,140,166,1) 100%);
  background-color: #08c4c4;
 }
 .line3 {
  max-width: 39px;
  width: 3vw;
  max-height: 7px;
  border-radius: 40px;
  
  height: 1vw;
  background-color: #12a1a1;background: rgb(2,0,36);
background: linear-gradient(90deg, rgb(0, 31, 36) 3%, rgba(18,88,102,1) 73%, rgba(70,140,166,1) 100%);
 }
 .line4 {
  max-width: 24px;
  max-height: 7px;
  width: 1.5vw;
  border-radius: 40px;
  height: 1vw;background: rgb(2,0,36);
background: linear-gradient(90deg, rgb(2, 42, 52) 3%, rgba(18,88,102,1) 73%, rgba(70,140,166,1) 100%);
  background-color: #096666;
 }
 .line {
   width: 100%;
   height: 2vw;
   bottom: 30vh;
   background-color: rgba(12, 104, 144, 0);
   box-shadow: rgba(0, 0, 0, 0.4) 0px 2px 4px, rgba(0, 0, 0, 0.3) 0px 7px 13px -3px, rgba(0, 0, 0, 0.2) 0px -3px 0px inset;
 }
 .getstarted {
   display: flex;
   justify-content: center;
   width: 60%;
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
     max-height: 160px;
     min-width: 250px;
   }
   .line {
     bottom: 55vh;
   }
   .hamburger {
    margin: 0px -30px;
    gap: 1.5px;
   }
   .text-code {
    font-size: 32px;
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
   height: 14vw;
   max-height: 160px;
   max-width: 470px;
   width: 55vw;
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
   font-size: max(60px);
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
 
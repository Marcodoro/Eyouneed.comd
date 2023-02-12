 
<script>
 
 export default {
   name: 'App',
   components: {

  },
   data() {
     return {
       login: false,
      }
  },
  methods: {
    open() {

    },
    clicked() {
      if (this.login == false) {
        this.login = true;
      } else {
        this.login = false
      }
    },
    submit() {
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
        <div class="login" @click="clicked()">
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
    <div class="rest" v-if="login == false">
       <div class="getstarted">
          <div class="learncode">
             <div class="text-code">Learn Web dev</div>
             <br>
               <button class="button-85" role="button"><span class="btn-text">Now and Free</span></button>
          </div>
       </div>
      </div>
       <div class="line" v-if="login == false"></div>
       <br>
          <div class="courses" v-if="login == false">
            <div class="border" v-if="login == false">
              <div class="fix" v-if="login == false">
                <div class="courses-text" v-if="login == false">
                  Courses that we offer &nbsp; 
                </div>
                <a href="" class="see-all">See all </a>
              </div>
              <br>
              <div class="scroll" v-if="login == false">
                <img src="https://via.placeholder.com/150/0000FF/808080 ?Text=PAKAINFO.com" alt="" height="250px">
                <img src="https://via.placeholder.com/150/0000FF/808080 ?Text=PAKAINFO.com" alt="" height="250px">
                <img src="https://via.placeholder.com/150/0000FF/808080 ?Text=PAKAINFO.com" alt="" height="250px">
                <img src="https://via.placeholder.com/150/0000FF/808080 ?Text=PAKAINFO.com" alt="" height="250px">
                <img src="https://via.placeholder.com/150/0000FF/808080 ?Text=PAKAINFO.com" alt="" height="250px">
              </div>
            </div>
      </div>  
      <div class="footer" v-if="login == false">
        <div class="down">
          <div class="icons">
             
          </div>
          <div class="icons">
             
          </div>
          <div class="icons">
             
           </div>
        </div>
      </div>    
      <template class="login" v-if="login == true">
           <div class="title">Login</div>
           <br>
           <br>
           <br>
           <br>
           <form netlify>
              <div class="name">
                 <input type="text" id="name" name="name" placeholder="Your Name" />
              </div>
              <div class="email">
                 <input type="email" id="email" name="email" placeholder="Your Email Address" />
              </div>
              <br>
              <div class="submit">
                <input class="button-36" type="submit" />
              </div>
           </form>
           <br>
           <br>
           <br><br><br><br><br><br><br><br><br><br>
           <div class="bottom">
            
           </div>
      </template> 
  </div> 
</template>
 <style>
 .bottom {
  width: 100%;
  height: 860px;
  background-color: black;
  background-image: linear-gradient(to bottom, rgb(20, 111, 111), rgb(39, 106, 113), black);
 }
/* CSS */
.button-36 {
  background-image: linear-gradient(92.88deg, #455EB5 9.16%, #5643CC 43.89%, #673FD7 64.72%);
  border-radius: 5px;
  border-style: none;
  box-sizing: border-box;
  color: #FFFFFF;
  cursor: pointer;
  flex-shrink: 0;
  font-family: "Inter UI","SF Pro Display",-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,Oxygen,Ubuntu,Cantarell,"Open Sans","Helvetica Neue",sans-serif;
  font-weight: 500;
  text-align: center;
  text-shadow: rgba(0, 0, 0, 0.25) 0 3px 8px;
  transition: all .5s;
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
  height: 9vw;
  width: 20vw;
}

.button-36:hover {
  box-shadow: rgba(80, 63, 205, 0.5) 0 1px 30px;
  transition-duration: .1s;
}

@media (min-width: 768px) {
  .button-36 {
    padding: 0 2.6rem;
  }
}
 ::placeholder {
  color: #000000;
 }
 #name,#email {
  width: 33vw;
  height: 3vw;
  min-height: 15px;
  min-width: 250px;
  border: black solid 2px;
  border-radius: 4px;
  max-height: 55px;
  max-width: 490px;
  background-image: linear-gradient(to right, #0d7478 9.16%, #5643CC);
 }
 form {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 100%;
  gap: 1vw;
  height: 100%;
  color: #ffffff;
  font-family: 'Roboto', sans-serif;
  font-size: 16px;
  font-weight: 400;
  letter-spacing: 1px;
  text-align: center;
 }
 .title {
  font-size: 4vw;
  font-weight: bolder;
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  text-align: center;
  display: flex;
  justify-content: center;
  background: #4DCF9B;
background: linear-gradient(to right, #4DCF9B 22%, #4A92FF 42%, #9B23CF 70%);
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;
 }
.footer {
  position: fixed;
  margin: 90% 0px;
  width: 100vw;
  height: 20px;
  background-color: rgb(179, 0, 0);
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px, rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px, rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
}
.down {
  position: fixed;
  margin: 90% 0px;
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px, rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px, rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
  width: 100vw;
  height: 20px;
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
   box-shadow: rgba(71, 123, 134, 0.295) 0px 19px 38px, rgba(27, 223, 174, 0.168) 0px 15px 12px;
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
   .title {
    font-size: 38px;
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
     min-height: 75px;
   }
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
    .button-36 {
      max-height: 60px;
      max-width: 150px;
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
 
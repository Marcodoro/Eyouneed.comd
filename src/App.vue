<script>

export default {
  data() {
    return {
       openvalue: Number,
    }
  },
  components: {

  },
  methods: {
    open() {
        this.openvalue = 50;
    }
  },
}

</script>

<template>
  <div class="page">
    <div class="menu">
       <div class="hamburger" @click="console.log(`clicked`)">
        <div class="wrappeer">
            <div class="line"></div>
            <div class="line2"></div>
            <div class="line3"></div>
            <div class="line4"></div>
        </div>
       </div>
       <div class="title">
           <div class="title-text">
             Eyouneed
           </div>
       </div>
       <div class="search">
          <div class="circle"></div>
          <div class="linee"></div>
       </div>
       <div class="login">
          <div class="login-text">
            Login
          </div>
       </div>
       <div class="home">
          <div class="home-text">
            Home
          </div>
       </div>
    </div>
    <br>
    <br>
    <br>
    <div class="under-menu">
      <div class="text">Shop</div>
      <div class="text">Learn to code</div>
      <div class="text">Code library</div>
      <div class="text">Register</div>
      <div class="text">Top flist</div>
    </div>
    <div class="open" :style="{width: openvalue}">

    </div>
    <br>
    <br>
    <div class="getstarted">
      <div class="getstarted-text">
        <div class="code-text">
          Learn Html
        </div>
        <span class="colorchange">
        </span>
        <div class="btn">
            <button class="button-64" role="button"><span class="text">
          Get started Now
            </span></button>
        </div>
    </div>
  </div>
  </div> 
</template>

<style scoped>
.line {
    width: 7.9vh;
    height: 1vh;
    background-color: #ffffff;
    border-radius: 55px;
}
.line2 {
    content: '';
    width: 6.4vh;
    height: 1vh;
    background-color: #ffffff;
    border-radius: 55px;
}
.line3{
    content: '';
    width: 5.0vh;
    height: 1vh;
    background-color: #ffffff;
    border-radius: 55px;
}
.line4{
    content: '';
    width:  3.0vh;
    height: 1vh;
    background-color: #ffffff;
    border-radius: 55px;
}
.wrappeer {
    display: flex;
    flex-direction: column;
    gap: 4px;
    margin: 3px 7px;
    justify-content: left;
}
@media only screen and (min-width: 1024px) {
    .wrappeer {
        margin: 6px -65%;
    }
}
@media only screen and (min-width: 1440px) {
    .wrappeer {
       margin: 6px -70%;
    }
}
@media only screen and (min-width: 720px) {
    .wrappeer {
        margin: 6px -30%;
    }
}
.getstarted {
  height: 30%;
  max-height: 300px;
  max-width: 700px;
  width: 70%;
  display: flex;
  justify-content: center;
  justify-self: center;
  align-content: center;
  left: 25%;
  position: absolute;
  align-items: center;
  flex-direction: column;
  font-weight: bolder;
  box-shadow: rgba(0, 0, 0, 0.25) 0px 14px 28px, rgba(0, 0, 0, 0.22) 0px 10px 10px;
}
.code-text {
  background: #00FF00;
  background: linear-gradient(to left, #00FF00 0%, #00FFFF 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-weight: bolder;
  display: flex;
  justify-content: center;
  font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  font-size: 5.2vh;
}
.menu {
  position: fixed;
  width: 100%;
  height: 8%;
  margin: 0px -10px;
  max-height: 70px;
  transition: hover 1.2s ease-in-out;
  background-color: rgba(31, 31, 31, 0.692);
  box-shadow: rgba(0, 0, 0, 0.3) 0px 19px 38px, rgba(0, 0, 0, 0.22) 0px 15px 12px;
  display: flex;
  justify-content: center;
  gap: 15px;
  background: #121FCF;
  background-image: linear-gradient(to right, #0b17b9 0%, #731716 100%);
  color: white;
}
.menu:hover {
  text-decoration: underline;;
}
.text {
  margin: .5vh 0px;
}
.under-menu {
  width: 97%;
  height: 2.5vh;
  margin: -5px 0px;
  display: flex;
  gap: 4%;
  flex-direction: row;
  background-image: linear-gradient(to right, rgb(60, 116, 117), rgb(117, 151, 171), rgb(53, 101, 109));
  box-shadow: rgba(0, 0, 0, 0.19) 0px 10px 20px, rgba(0, 0, 0, 0.23) 0px 6px 6px;
  border-radius: 2px;
  font-weight: bolder;
  font-size: 14px;
  font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  background: linear-gradient(to right, #0b17b9 0%, #731716 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
/* CSS */
.button-64 {
  background-image: linear-gradient(144deg,#AF40FF, #5B42F3 50%,#00DDEB);
  border: 0;
  border-radius: 8px;
  box-shadow: rgba(151, 65, 252, 0.2) 0 15px 30px -5px;
  color: #FFFFFF;
  display: flex;
  font-family: Phantomsans, sans-serif;
  font-size: 4.5vh;
  justify-content: center;
  height: 9vh;
  width: 30vh;
  max-height: 200px;
  max-width: 400px;
  text-decoration: none;
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
  white-space: nowrap;
  font-weight: bolder;
  display: flex;
  justify-content: center;
  flex-direction: column;
  cursor: pointer;
}

.button-64:active,
.button-64:hover {
  outline: 0;
}

.button-64 span {
  background-color: rgb(5, 6, 45);
  border-radius: 6px;
  display: flex;
  justify-content: center;
  flex-direction: column;
  width: 100%;
  height: 99%;
  transition: 300ms;
  font-size: 2.7vh;
}

.button-64:hover span {
  background: none;
}

@media (min-width: 768px) {
  .button-64 {
    font-size: 24px;
    min-width: 196px;
  }
}
.under-menu:hover {
  filter: blur(0.2px);
}
.open {
  height: 1000px;
  background-color: black;
  position: fixed;
}
.menu:hover {
  background-color: rgb(22, 22, 22);
  box-shadow: rgba(0, 0, 0, 0.3) 0px 19px 48px, rgba(0, 0, 0, 0.22) 0px 15px 12px;
}
.hamburger {
  border: 2px transparent solid;
  width: 10%;
  height: 48px;
  display: flex;
  justify-content: left;
  margin: 0px 0px;
}
.login {
  border: 2px transparent solid;
  font-size: 3.5vh;
  width: 20%;
  height: 47px;
  font-weight: bolder;
  color: white;
  display: flex;
  justify-content: center;
  flex-direction:column;
  font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}

.search {
  border: 2px transparent solid;
  width: 10%;
  height: 48px;
  font-size: 3.5vh;
  display: flex;
  flex-direction: columns;
  display: flex;
  justify-content: center;
  flex-direction:column;
  justify-content: center;
}
.home {
  border: 2px transparent solid;
  width: 20%;
  height: 48px;
  display: flex;
  justify-content: center;
  flex-direction:column;
  font-weight: bolder;
  font-size: 3.5vh;
  color: white;
  font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}
.title {
  border: 2px transparent solid;
  width: 20%;
  height: 48px;
  font-size: 3.5vh;
  display: flex;
  justify-content: center;
  flex-direction:column;
  font-weight: bolder;
  color: white;
  font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}
.title-text {
  margin: 13px 0px;
}
.home-text {
  margin: 13px 0px;
}
.login-text {
  margin: 13px 0px;
}
.circle {
  width: 17px;
  height: 17px;
  border: solid 2.5px white;
  border-radius: 100%;
  margin: 4px 0px;
}
.linee {
  width: 20px;
  height: 4px;
  border-radius: 55px;
  background-color: white;
  margin: 24px 0%;
  transform: rotate(30deg);
}
body {
  overflow-x: hidden;
  overflow-y: hidden;
  max-height: 1300px;
}

@media only screen and (max-width: 412px) {
  .menu {
      width: 100%;
      height: 42px;
    }
  .hamburger {
      width: 100%;
      height: 42px;
    }
  .login {
      width: 100%;
      height: 42px;
    }
  .search {
      width: 100%;
      height: 42px;
    }
  .home {
      width: 100%;
      height: 42px;
    }
  .title {
      width: 100%;
      height: 42px;
    }
    .getstarted {
      left: 15%;
    }
.title-text {
  margin: 8px 00px;
  font-size: 19px;
}
.home-text {
  margin: 8px 00px;
  font-size: 19px;
}
.login-text {
  margin: 8px 00px;
  font-size: 19px;
}
.menu {
  width: 96%;
}
}
@media only screen and (min-width: 1080px) {
  .getstarted {
    left: 15%;
  }
}
@media only screen and (min-width: 1024px) {
  .getstarted {
    left: 12.5%;
  }
}
@media only screen and (min-width: 1880px) {
  .getstarted {
    left: 30%;
  }
}
</style>

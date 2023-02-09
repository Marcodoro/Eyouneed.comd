<script>
import Hamburger from './components/icons/Hamburger.vue';

export default {
  data() {
    return {
       openvalue: Number,
    }
  },
  components: {
    Hamburger,
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
           <Hamburger />
       </div>
       <div class="title">
           <div class="title-text">
             Eyouneed
           </div>
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
       <div class="search">

       </div>
    </div>
    <div class="open" :style="{width: openvalue}">

    </div>
  </div>
</template>

<style scoped>
.menu {
  width: 100%;
  height: 50px;
  transition: hover 1.2s ease-in-out;
  background-color: rgb(31, 31, 31);
  box-shadow: rgba(0, 0, 0, 0.3) 0px 19px 38px, rgba(0, 0, 0, 0.22) 0px 15px 12px;
  display: flex;
  justify-content: center;
  gap: 15px;
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
  border: 2px red solid;
  width: 10%;
  height: 48px;
  display: flex;
  justify-content: left;
  margin: 0px 0px;
}
.login {
  border: 2px red solid;
  width: 20%;
  height: 47px;
  font-weight: bolder;
  color: white;
  font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif
}
.search {
  border: 2px red solid;
  width: 10%;
  height: 48px;
}
.home {
  border: 2px red solid;
  width: 20%;
  height: 48px;
  font-weight: bolder;
  color: white;
  font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif
}
.title {
  border: 2px red solid;
  width: 20%;
  height: 48px;
  font-weight: bolder;
  color: white;
  font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif
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

@media only screen and (max-width: 412px) {
  .menu {
      width: 100%;
      height: 32px;
    }
  .hamburger {
      width: 100%;
      height: 32px;
    }
  .login {
      width: 100%;
      height: 32px;
    }
  .search {
      width: 100%;
      height: 32px;
    }
  .home {
      width: 100%;
      height: 32px;
    }
  .title {
      width: 100%;
      height: 32px;
    }
.title-text {
  margin: 6px 00px;
}
.home-text {
  margin: 6px 00px;
}
.login-text {
  margin: 6px 00px;
}
}
</style>

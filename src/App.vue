<template>
  <div v-if="show" class="container-cus">
    <!-- animate background start -->
    <div class="animate-bg">
      <span class="bubble" style="--d:11;"></span>
      <span class="bubble" style="--d:27;"></span>
      <span class="bubble" style="--d:8;"></span>
      <span class="bubble" style="--d:20;"></span>
      <span class="bubble" style="--d:13;"></span>
      <span class="bubble" style="--d:19;"></span>
      <span class="bubble" style="--d:30;"></span>
      <span class="bubble" style="--d:28;"></span>
      <span class="bubble" style="--d:7;"></span>
      <span class="bubble" style="--d:15;"></span>
      <span class="bubble" style="--d:22;"></span>
      <span class="bubble" style="--d:5;"></span>
      <span class="bubble" style="--d:14;"></span>
      <span class="bubble" style="--d:28;"></span>
      <span class="bubble" style="--d:17;"></span>
      <span class="bubble" style="--d:7;"></span>
      <span class="bubble" style="--d:16;"></span>
      <span class="bubble" style="--d:25;"></span>
      <span class="bubble" style="--d:30;"></span>
      <span class="bubble" style="--d:11;"></span>
      <span class="bubble" style="--d:19;"></span>
      <span class="bubble" style="--d:7;"></span>
      <span class="bubble" style="--d:23;"></span>
      <span class="bubble" style="--d:27;"></span>
      <span class="bubble" style="--d:13;"></span>
      <span class="bubble" style="--d:12;"></span>
      <span class="bubble" style="--d:28;"></span>
      <span class="bubble" style="--d:7;"></span>
      <span class="bubble" style="--d:16;"></span>
      <span class="bubble" style="--d:19;"></span>
      <span class="bubble" style="--d:8;"></span>
      <span class="bubble" style="--d:28;"></span>
      <span class="bubble" style="--d:17;"></span>
      <span class="bubble" style="--d:24;"></span>
      <span class="bubble" style="--d:30;"></span>
      <span class="bubble" style="--d:11;"></span>
    </div>
    <!-- animate background end -->
    <div class="row upper-layer">

      <!-- page title start -->
      <div class="col-12 head-cus">
        <h1 class="text-uppercase text-center font-bold mt-cus title-cus">
          {{ title }}
        </h1>
        <div class="mx-auto bg-primary line-cus"></div>
      </div>
      <!-- page title end -->

      <div class="row body-cus">
        <!-- router-view start -->
        <div class="col-12 col-lg-6 order-last order-lg-0">
          <router-view />
        </div>
        <!-- router-view end -->

        <!-- router-links start-->
        <div class="col-12 col-lg-6 my-3 my-lg-0">
          <LinksComponent @chg-title="chgTitle" />
        </div>
        <!-- router-links end -->

      </div>
    </div>
  </div>

  <div v-else class="loader">
    <img src="@/assets/loader.gif" alt="">
  </div>
  <!-- <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </nav>
  <router-view/> -->
</template>

<script>
import LinksComponent from './components/LinksComponent.vue'

export default {
  data() {
    return {
      title: 'home',
      show: false
    }
  },
  components: {
    LinksComponent
  },
  mounted() {
    document.onreadystatechange = () => {
      if (document.readyState === "complete") {
        this.show = true;
      }
    }
  },
  methods: {
    chgTitle(title) {
      this.title = title;
    }
  },
}
</script>

<style lang="scss">
$primary: #70e2ff;
$secondary: #3A3A3A;
$bgcustom: #25282C;
$bgloader: #1f242c;

$carousel-control-color: #000000;

$carousel-indicator-width: 50px;
$carousel-indicator-height: 10px;
$carousel-indicator-active-bg: #000000;

@import '../node_modules/bootstrap/scss/bootstrap';

.loader {
  width: 100%;
  height: 100vh;
  background: $bgloader;
  display: grid;
  place-items: center;
}

.loader img {
  width: 50%;
}

.line-cus {
  width: 200px;
  height: 5px;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  overflow: hidden;
}

.container-cus {
  width: 100%;
  min-height: 100vh;
  position: relative;
  background: #25282c;
  overflow: hidden;
  color: white;
}

.upper-layer {
  position: relative;
  z-index: 1;
  height: 100vh;
}

.head-cus {
  height: 20%;
}

.body-cus {
  height: 80%;
  grid-auto-flow: dense;
}

.animate-bg {
  position: absolute;
  width: 100%;
  height: 100%;
  display: flex;
}

.animate-bg .bubble {
  width: 30px;
  height: 30px;
  background: #4fc3dc;
  margin: 0 4px;
  border-radius: 50%;
  box-shadow: 0 0 0 10px #4fc3dc44,
    0 0 50px #4fc3dc,
    0 0 100px #4fc3dc;
  animation: bubble 15s linear infinite;
  animation-duration: calc(125s / var(--d));
  flex-shrink: 0;
}

.animate-bg .bubble:nth-of-type(even) {
  background: #ff2d75;
  box-shadow: 0 0 0 10px #ff2d7544,
    0 0 50px #ff2d75,
    0 0 100px #ff2d75;
}

@keyframes bubble {
  0% {
    transform: translateY(100vh) scale(0);
  }

  100% {
    transform: translateY(-10vh) scale(1);
  }
}

ul li {
  list-style: none;
  width: 200px;
  height: 50px;
  background: #474747;
  padding: 0 20px;
  line-height: 50px;
  cursor: pointer;
  transform: skewY(-15deg) translateX(0);
  transition: all 0.5s;

  position: relative;
  z-index: var(--i);
}

ul li:hover {
  background: $primary;
  transform: skewY(-15deg) translateX(50px);
}

ul li::before {
  content: '';

  width: 50px;
  height: 100%;
  position: absolute;
  top: 0;
  left: -50px;
  background: #3a3a3a;
  transform-origin: right;
  transform: skewY(45deg);
  transition: all 0.5s;
}

ul li:hover::before {
  background: #66c5dd;
}

ul li::after {
  content: '';

  width: 100%;
  height: 100%;
  position: absolute;
  top: -100%;
  left: 0;
  background: #424242;
  transform-origin: bottom;
  transform: skewX(45deg);
  transition: all 0.5s;
}

ul li:hover::after {
  background: #64c8e0;
}

ul li a {
  width: 100%;
  height: 100%;
  display: inline-block;
  color: #b6b6b6;
  font-size: 1.5rem;
  text-decoration: none;
}

ul li:last-child {
  box-shadow: 0 120px 30px #00000080;
}

ul li:hover a {
  color: #ffffff;
}

.mt-cus {
  margin-top: 100px !important;
}

@media screen and (max-width: 1480px) {
  .mt-cus {
    margin-top: 40px !important;
  }
}

@media screen and (max-width: 500px) {
  .mt-cus {
    margin-top: 10px !important;
  }

  .animate-bg .bubble {
    width: 15px;
    height: 15px;
    margin: 0 2px;
    border-radius: 50%;
    box-shadow: 0 0 0 5px #4fc3dc44,
      0 0 25px #4fc3dc,
      0 0 50px #4fc3dc;
  }

  .animate-bg .bubble:nth-of-type(even) {
    box-shadow: 0 0 0 5px #ff2d7544,
      0 0 25px #ff2d75,
      0 0 50px #ff2d75;
  }

  ul li {
    width: 100px;
    height: 25px;
    padding: 0 10px;
    line-height: 25px;
    transform: skewY(-15deg) translateX(0);
  }

  ul li:hover {
    transform: skewY(-15deg) translateX(25px);
  }

  ul li::before {
    width: 25px;
    left: -25px;
  }

  ul li a {
    font-size: 16px;
  }

  ul li:last-child {
    box-shadow: 0 30px 15px #00000080;
  }

  .title-cus {
    font-size: 24px;
  }

  .line-cus {
    width: 150px;
    height: 3px;
  }

  .head-cus {
    height: 10vh;
  }

  .body-cus {
    height: 90vh;
  }
}
</style>

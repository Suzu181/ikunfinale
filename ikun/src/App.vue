<template>
  <div>
    <nav class="navbar" id="main-nav">
      <div class="header">
        <h1>IKUN</h1>
        <img class="navkun" src="./assets/navbarKun.png" alt="" />
      </div>
      <button><router-link to="/">Home</router-link></button>
      <button><router-link to="/about">Gallery1</router-link></button>
      <button><router-link to="/gallery2">Gallery2</router-link></button>
    </nav>
  </div>
  <RouterView />
</template>

<script>
import { RouterLink, RouterView } from "vue-router";

export default {
  components: {},
  setup() {
    return {};
  },
};
</script>

<style scoped>
.navbar {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  height: 10rem;
  overflow: hidden;
  background-color: #ffc0cb;
  position: fixed; /* Set the navbar to fixed position */
  top: 0; /* Position the navbar at the top of the page */
  width: 100%; /* Full width */
  z-index: 10;
}
.header {
  display: flex;
  flex-direction: row;
  text-align: center;
  width: 20rem;
  height: 10rem;
}
button {
  background-color: white;
  font-size: 1.5rem;
  margin-top: 3rem;
  height: 4rem;
  width: 9rem;

  border-radius: 2rem;
}
.parallel {
  margin-top: 10rem;
}
h1 {
  font-size: 4rem;
  color: white;
}
a {
  text-decoration: none;
  color: black;
}
.bgimg-1,
.bgimg-2,
.bgimg-3,
.bgimg-4 {
  position: relative;
  opacity: 0.65;
  background-attachment: fixed;
  background-position: center;

  background-size: cover;
}

.bgimg-2 {
  background-image: url("./assets/parallelfirst.jpg");
  min-height: 600px;
}

.bgimg-3 {
  background-image: url("./assets/parallelthird.jpg");
  min-height: 400px;
}

#bgimg-2 {
  background-image: url("./assets/IMG_8284.jpg");
}

.caption {
  position: absolute;
  left: 0;
  top: 50%;
  width: 100%;
  text-align: center;
  color: #000;
}

.caption span.border {
  background-color: #111;
  color: #fff;
  padding: 18px;
  font-size: 25px;
  letter-spacing: 10px;
}

h3 {
  letter-spacing: 5px;
  text-transform: uppercase;
  font: 20px "Lato", sans-serif;
  color: #111;
}

#slider figure img {
  float: left;
  width: 400px;
  height: 400px;
  gap: 20px;
  object-fit: cover;
}
figure {
  display: grid;
  grid-template-columns: auto auto auto auto auto auto auto auto auto auto auto;
  gap: 2rem;
}

.rotate {
  display: flex;
  flex-direction: row;
}
#slider {
  overflow: hidden;
}
#slider figure {
  position: relative;
  width: 500%;
  margin: 0;
  left: 0;
  animation: 20s slider infinite ease-in-out;
}
@keyframes slider {
  0% {
    left: 0;
  }
  20% {
    left: 0;
  }
  25% {
    left: -100%;
  }
  45% {
    left: -100%;
  }
  50% {
    left: -200%;
  }
  70% {
    left: -200%;
  }
  75% {
    left: -300%;
  }
  95% {
    left: -300%;
  }
  100% {
    left: -400%;
  }
}
.box {
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: white;

  height: 500px;
  width: 800px;
  border-radius: 2rem;
}
.rotatepic {
  float: left;
  width: 400px;
  height: 400px;
  gap: 20px;
  object-fit: cover;
}
</style>

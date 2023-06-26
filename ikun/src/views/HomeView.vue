<template>
  <div>
    <div class="parallel">
      <div class="bgimg-2">
        <div class="caption">
          <span
            class="border"
            style="
              background-color: transparent;
              font-size: 25px;
              color: #f7f7f7;
            "
            >SCROLL DOWN</span
          >
        </div>
      </div>
      <div style="position: relative">
        <div
          style="
            color: #ddd;
            background-color: #ffc0cb;
            text-align: center;
            padding: 50px 80px;
            text-align: justify;
            height: 400px;
          "
        >
          <div id="slider">
            <figure class="rotate">
              <img class="slidepic" src="../assets/slider1.jpg" alt="slider1" />
              <img class="slidepic" src="../assets/slider2.jpg" alt="slider2" />
              <img class="slidepic" src="../assets/slider3.jpg" alt="slider3" />
              <img class="slidepic" src="../assets/slider4.jpg" alt="slider4" />
              <img class="slidepic" src="../assets/slider5.jpg" alt="slider5" />
              <img class="slidepic" src="../assets/slider6.jpg" alt="slider6" />
              <img class="slidepic" src="../assets/slider7.jpg" alt="slider7" />
              <img class="slidepic" src="../assets/slider8.jpg" alt="slider8" />
              <img class="slidepic" src="../assets/slider9.jpg" alt="slider9" />
              <img
                class="slidepic"
                src="../assets/slider10.jpg"
                alt="slider10"
              />
              <img
                class="slidepic"
                src="../assets/slider11.jpg"
                alt="slider11"
              />
              <img
                class="slidepic"
                src="../assets/slider12.jpg"
                alt="slider12"
              />
              <img
                class="slidepic"
                src="../assets/slider13.jpg"
                alt="slider13"
              />
            </figure>
          </div>
        </div>
      </div>

      <div class="bgimg-3"></div>

      <div style="position: relative">
        <div
          style="
            color: #ddd;
            background-color: #ffc0cb;
            text-align: center;
            padding: 50px 80px;
            text-align: justify;
          "
        >
          <div id="rotater">
            <figure class="rotate">
              <div class="box">
                <img
                  class="rotatepic"
                  src="../assets/rotate1.jpg"
                  alt="slider1"
                />
              </div>
              <div class="box">
                <img
                  class="rotatepic"
                  src="../assets/rotate2.jpg"
                  alt="slider2"
                />
              </div>
              <div class="box">
                <img
                  class="rotatepic"
                  src="../assets/rotate3.jpg"
                  alt="slider3"
                />
              </div>
            </figure>
          </div>
        </div>
      </div>

      <div class="bgimg-2" id="bgimg-2">
        <div class="caption">
          <span
            class="border"
            style="background-color: transparent; font-size: 25px"
            >SCROLL UP</span
          >
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
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

body,
html {
  height: 100%;
  margin: 0;
  font: 400 15px/1.8 "Lato", sans-serif;
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
  background-image: url("../assets/parallelfirst.jpg");
  min-height: 600px;
}

.bgimg-3 {
  background-image: url("../assets/parallelthird.jpg");
  min-height: 400px;
}

#bgimg-2 {
  background-image: url("../assets/IMG_8284.jpg");
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

<template>
  <div>
    <div id="gallery">
      <div class="gallery-wrapper">
        <div class="gallery-container h-2">
          <div class="gallery-item">
            <div class="image">
              <img
                src="https://e1.pxfuel.com/desktop-wallpaper/471/37/desktop-wallpaper-cai-xukun.jpg"
              />
            </div>
          </div>
        </div>

        <div class="gallery-container">
          <div class="gallery-item">
            <div class="image">
              <img src="https://wallpapercave.com/wp/wp4473679.jpg" />
            </div>
          </div>
        </div>

        <div class="gallery-container">
          <div class="gallery-item">
            <div class="image">
              <img
                src="https://e1.pxfuel.com/desktop-wallpaper/174/726/desktop-wallpaper-108-about-cai-xukun.jpg"
              />
            </div>
          </div>
        </div>

        <div class="gallery-container h-2 w-3">
          <div class="gallery-item">
            <div class="image">
              <img
                src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d5/Cai_Xukun_in_2018.jpg/800px-Cai_Xukun_in_2018.jpg"
              />
            </div>
          </div>
        </div>

        <div class="gallery-container">
          <div class="gallery-item">
            <div class="image">
              <img
                src="https://i.pinimg.com/originals/3c/92/b8/3c92b875db450d0d859ed249a21250e3.png"
              />
            </div>
          </div>
        </div>

        <div class="gallery-container">
          <div class="gallery-item">
            <div class="image">
              <img
                src="https://pm1.narvii.com/6819/3a8a62b8ff7322c30b8669b870954b9f71137192v2_00.jpg"
              />
            </div>
          </div>
        </div>

        <div class="gallery-container">
          <div class="gallery-item">
            <div class="image">
              <img
                src="https://cdn.idntimes.com/content-images/community/2020/10/96747088-888397534956294-2195934735108390904-n-1e0a7921201bdcae4e9fb38de016a305.jpg"
              />
            </div>
          </div>
        </div>

        <div class="gallery-container w-2 h-3">
          <div class="gallery-item">
            <div class="image">
              <img
                src="https://64.media.tumblr.com/00e87f4744c78559b2ce469080ed5db9/tumblr_plhyoi4qLy1x9c3cwo1_1280.jpg"
              />
            </div>
          </div>
        </div>

        <div class="gallery-container">
          <div class="gallery-item">
            <div class="image">
              <img
                src="https://www.cpophome.com/wp-content/uploads/2020/11/Cai-Xukun-1.jpg"
              />
            </div>
          </div>
        </div>

        <div class="gallery-container">
          <div class="gallery-item">
            <div class="image">
              <img src="https://pbs.twimg.com/media/EjZmL8BU8AAGOfu.jpg" />
            </div>
          </div>
        </div>

        <div class="gallery-container w-2 h-3">
          <div class="gallery-item">
            <div class="image">
              <img src="https://pbs.twimg.com/media/EUnJd_4UcAcqQ4J.jpg" />
            </div>
          </div>
        </div>

        <div class="gallery-container">
          <div class="gallery-item">
            <div class="image">
              <img src="https://wallpapercave.com/wp/wp4473673.jpg" />
            </div>
          </div>
        </div>

        <div class="gallery-container">
          <div class="gallery-item">
            <div class="image">
              <img
                src="https://pbs.twimg.com/media/DoVOfQ3WsAA5rwJ?format=jpg&name=large"
              />
            </div>
          </div>
        </div>

        <div class="gallery-container">
          <div class="gallery-item">
            <div class="image">
              <img src="https://i.imgur.com/H2ja8hm.jpg" />
            </div>
          </div>
        </div>

        <div class="gallery-container">
          <div class="gallery-item">
            <div class="image">
              <img
                src="https://p9.toutiaoimg.com/origin/tos-cn-i-qvj2lq49k0/6aa8b5da20cc4276ba688526f5115a89?from=pc"
              />
            </div>
          </div>
        </div>

        <div class="gallery-container">
          <div class="gallery-item">
            <div class="image">
              <img
                src="https://p1-tt.byteimg.com/origin/pgc-image/e82bfc0e16e743c797e06c964075e6a4.jpg"
              />
            </div>
          </div>
        </div>

        <div class="gallery-container w-2">
          <div class="gallery-item">
            <div class="image">
              <img
                src="https://pbs.twimg.com/media/DoVOZQBXkAArbAH.jpg:large"
              />
            </div>
          </div>
        </div>

        <div class="gallery-container">
          <div class="gallery-item">
            <div class="image">
              <img
                src="https://64.media.tumblr.com/a7661d864956e9f27cdf26e2f8d44fcf/tumblr_plhdrsLFez1x9c3cwo1_1280.jpg"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "GalleryTwo",
  components: {},
};
</script>

<style scoped>
.gallery-wrapper {
  margin-top: 10rem;
  padding: 2rem 7rem;
  display: grid;
  justify-content: center;
  grid-template-columns: repeat(5, 1fr);
  grid-auto-rows: auto;
  grid-gap: 1rem;
  grid-auto-flow: dense;
}

.gallery-item {
  width: 100%;
  height: 100%;
  position: relative;
  filter: drop-shadow(2px 2px 3px #333);
}

.gallery-item .image {
  width: 100%;
  height: 100%;
  overflow: hidden;
}

.gallery-item .image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: 50% 50%;
  cursor: pointer;
  transition: all 400ms ease-in;
  transform: scale(1);
}

.gallery-item .image img:hover {
  transform: scale(1.1);
}

.w-1 {
  grid-column: span 1;
}
.w-2 {
  grid-column: span 2;
}
.w-3 {
  grid-column: span 3;
}
.w-4 {
  grid-column: span 4;
}
.w-5 {
  grid-column: span 5;
}

.h-1 {
  grid-row: span 1;
}
.h-2 {
  grid-row: span 2;
}
.h-3 {
  grid-row: span 3;
}
.h-4 {
  grid-row: span 4;
}
.h-5 {
  grid-row: span 5;
}

/* ***** LIGHTBOX EFFECT ***** */

#lightbox {
  position: fixed;
  z-index: 1000;
  top: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.92);
  display: none;
}

#lightbox.active {
  display: flex;
  justify-content: center;
  align-items: center;
}

#lightbox img {
  max-width: 90%;
  max-height: 80%;
  padding: 4px;
  /* border-radius: 1%; */
  /* background-color: white; */
  border: 0.2px solid silver;
}

/* Generic Styles */

html {
  height: 100%;
  font-family: sans-serif;
  font-size: 1vw;
  scroll-behavior: smooth;
}

body {
  height: 100vh;
  min-width: 100vw;
  margin: 0;
  padding: 0;
}

@media only screen and (max-width: 800px) {
  .gallery-wrapper {
    grid-template-columns: repeat(2, 2fr);
    grid-template-rows: 1fr;
    grid-gap: 2;
    grid-auto-flow: dense;
  }
  .gallery-container:nth-child(3n + 2) {
    grid-column: 1 / span 2;
    grid-row-end: span 2;
  }

  .gallery-container:nth-child(4n + 3) {
    grid-column: 2 / span 1;
    grid-row-end: span 2;
  }

  /*  reseting the css for the class within the divs to show a different way to achieve grid control using the nth childs*/
  .w-1,
  .w-2,
  .w-3,
  .w-4,
  .w-5 {
    grid-column: span 1;
  }

  .h-1,
  .h-2,
  .h-3,
  .h-4,
  .h-5 {
    grid-row: span 1;
  }
}

@media only screen and (max-width: 400px) {
  /* An example to use combined with flex but could also be grids with different repetition of columns  */
  .gallery-wrapper {
    display: flex;
    flex-direction: column;
    flex: wrap;
    gap: 2.5rem;
    margin: 5rem;
  }
}
</style>

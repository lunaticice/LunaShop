<template>
  <!-- Hero Section Begin -->
  <section class="hero-section">
    <carousel class="hero-items" :items="1" :nav="false" :autoplay="true">
      <div class="single-hero-items set-bg" style="background-image: url('/images/art-transparent.png')">
        <div class="container">
          <div class="row">
            <div class="col-lg-5">
              <span>art</span>
              <h1>Home for creatives</h1>
              <p>Find your best art tool here!</p>
              <a href="#" class="primary-btn">Shop Now</a>
            </div>
          </div>
        </div>
      </div>

      <div class="single-hero-items set-bg" style="background-image: url('/images/game-transparent.png')">
        <div class="container">
          <div class="row">
            <div class="col-lg-5">
              <span>game</span>
              <h1>Fulfill your gaming needs</h1>
              <p>Find your gaming kit here!</p>
              <a href="#" class="primary-btn">Shop Now</a>
            </div>
          </div>
        </div>
      </div>

      <div class="single-hero-items set-bg" style="background-image: url('/images/hobby-transparent.png')">
        <div class="container">
          <div class="row">
            <div class="col-lg-5">
              <span>hobby</span>
              <h1>Home for hobbyist</h1>
              <p>Find your goods here!</p>
              <a href="#" class="primary-btn">Shop Now</a>
            </div>
          </div>
        </div>
      </div>

      <div class="single-hero-items set-bg" style="background-image: url('/images/music-transparent.png')">
        <div class="container">
          <div class="row">
            <div class="col-lg-5">
              <span>music</span>
              <h1>Music to your heart content</h1>
              <p>Find your musical instrument here!</p>
              <a href="#" class="primary-btn">Shop Now</a>
            </div>
          </div>
        </div>
      </div>

      <div class="single-hero-items set-bg" style="background-image: url('/images/technology-transparent.png')">
        <div class="container">
          <div class="row">
            <div class="col-lg-5">
              <span>technology</span>
              <h1>Geeks & Developer Zone</h1>
              <p>Find your desired technology here!</p>
              <a href="#" class="primary-btn">Shop Now</a>
            </div>
          </div>
        </div>
      </div>
    </carousel>
  </section>
  <!-- Hero Section End -->
</template>

<script>
import carousel from "vue-owl-carousel";

export default {
  name: "HeroLunaShop",
  components: {
    carousel
  }
};
</script>
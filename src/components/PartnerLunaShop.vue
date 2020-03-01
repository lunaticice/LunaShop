<template>
  <!-- Partner Logo Section Begin -->
  <div class="partner-logo">
    <div class="container">
      <carousel class="logo-carousel" :items="4" :nav="false" :autoplay="true" :loop="true" :dots="false">
        <div class="logo-item">
          <div class="tablecell-inner">
            <img src="images/logo.png" alt />
          </div>
        </div>
        <div class="logo-item">
          <div class="tablecell-inner">
            <img src="img/logo-carousel/logo-2.png" alt />
          </div>
        </div>
        <div class="logo-item">
          <div class="tablecell-inner">
            <img src="img/logo-carousel/logo-3.png" alt />
          </div>
        </div>
        <div class="logo-item">
          <div class="tablecell-inner">
            <img src="img/logo-carousel/logo-4.png" alt />
          </div>
        </div>
        <div class="logo-item">
          <div class="tablecell-inner">
            <img src="img/logo-carousel/logo-5.png" alt />
          </div>
        </div>
      </carousel>
    </div>
  </div>
  <!-- Partner Logo Section End -->
</template>

<script>

import carousel from "vue-owl-carousel";

export default {
  name: "PartnerLunaShop",
  components: {
    carousel
  }  
}
</script>

<style scoped>
img {
  width: 100px;
  height: 100px;
}
</style>
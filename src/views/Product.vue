<template>
  <div class="product">
    <HeaderLunaShop />
    <!-- Breadcrumb Section Begin -->
    <div class="breacrumb-section text-left">
      <div class="container">
        <div class="row">
          <div class="col-lg-12">
            <div class="breadcrumb-text product-more">
              <router-link to="/">
                <i class="fa fa-home"></i> Home
              </router-link>
              <span>Detail</span>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- Breadcrumb Section Begin -->

    <!-- Product Shop Section Begin -->
    <section class="product-shop spad page-details">
      <div class="container">
        <div class="row">
          <div class="col-lg-12">
            <div class="row">
              <div class="col-lg-6">
                <div class="product-pic-zoom">
                  <img class="product-big-img" :src= "defaultImage" alt />
                </div>
                <div class="product-thumbs">
                  <carousel :dots="false" :nav="false"  class="product-thumbs-track ps-slider">
                    <div class="pt" @click="changeImage(carouselImage[0])" :class="carouselImage[0] == defaultImage ? 'active' : '' ">
                      <img src="images/products/samsung-galaxy-note-10-plus-thumb.jpg" alt />
                    </div>

                    <div class="pt" @click="changeImage(carouselImage[1])" :class="carouselImage[1] == defaultImage ? 'active' : '' ">
                      <img src="images/products/samsung-galaxy-note-10-plus-1.jpg" alt />
                    </div>

                    <div class="pt" @click="changeImage(carouselImage[2])" :class="carouselImage[2] == defaultImage ? 'active' : '' ">
                      <img src="images/products/samsung-galaxy-note-10-plus-2.jpg" alt />
                    </div>
                  </carousel>
                </div>
              </div>
              <div class="col-lg-6">
                <div class="product-details text-left">
                  <div class="pd-title">
                    <span>smartphone</span>
                    <h3>Samsung Galaxy Note10+ 256GB - Aura Black</h3>
                  </div>
                  <div class="pd-desc">
                    <p>Samsung Galaxy Note10+ 256GB - Aura Black</p>
                    <p>Specification Details</p>
                    <p>Display size: 6.8 inch, 1440 x 3040 pixels, 19:9 ratio, Dynamic AMOLED capacitive touchscreen, 16M colors</p>
                    <p>Memory: RAM 12 GB, ROM 256 GB, microSD up to 1 TB</p>
                    <p>Operating System: Android 9.0 (Pie); One UI</p>
                    <p>CPU: Exynos 9825 (7 nm), Octa-core (2x2.73 GHz Mongoose M4 & 2x2.4 GHz Cortex-A75 & 4x1.9 GHz Cortex-A55)</p>
                    <p>GPU: Mali-G76 MP12</p>
                    <p>Rear Camera: Triple 12 MP, f/1.5-1.8-2.4, 27mm (wide), 1/2.55"", 1.4Âµm, Dual Pixel PDAF, OIS. 12 MP, f/2.1, 52mm (telephoto), 1/3.6"", 1.0Âµm, AF, OIS, 2x optical zoom, 16 MP, f/2.2, 12mm (ultrawide), 1.0Âµm, TOF 3D VGA camera</p>
                    <p>Front Camera: Single 10 MP, f/2.2, 26mm (wide), 1.22Âµm, Dual Pixel PDAF</p>
                    <p>SIM: Dual SIM (Nano-SIM, dual stand-by)<p>
                    <p>Battery: Non-removable Li-Ion 4300 mAh
                    <p>Weight: 196 gram</p>
                    <h4>Rp 16.099.000</h4>
                  </div>
                  <div class="quantity">
                    <router-link to="/cart" class="primary-btn pd-cart">Add To Cart</router-link>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- Product Shop Section End -->
    <RelatedProducts />
    <FooterLunaShop />
  </div>
</template>

<script>
// @ is an alias to /src
import HeaderLunaShop from "@/components/HeaderLunaShop.vue";
import RelatedProducts from "@/components/RelatedProducts.vue";
import FooterLunaShop from "@/components/FooterLunaShop.vue";

import carousel from "vue-owl-carousel";

export default {
  name: "product",
  components: {
    HeaderLunaShop,
    RelatedProducts,
    FooterLunaShop,
    carousel
  },
  data() {
      return {
          defaultImage: "images/products/samsung-galaxy-note-10-plus-thumb.jpg",
          carouselImage: [
              "images/products/samsung-galaxy-note-10-plus-thumb.jpg",
              "images/products/samsung-galaxy-note-10-plus-1.jpg",
              "images/products/samsung-galaxy-note-10-plus-2.jpg"
          ]
      }
  },
  methods: {
      changeImage(urlImage) {
          this.defaultImage = urlImage;
      }
  }
};
</script>

<style scoped>
.product-thumbs .pt {
    margin-right: 14px;
}
</style>

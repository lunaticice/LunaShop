<template>
  <!-- Women Banner Section Begin -->
  <section class="women-banner spad">
    <div class="container-fluid">
      <div class="row">
        <div class="col-lg-12 mt-5">
          <carousel class="product-slider" :items="3" :nav="false" :autoplay="true" :dots="false">
            <div class="product-item">
              <div class="pi-pic">
                <img src="images/products/wacom-cintiq-dtc-330-thumb.jpg" alt />
                <ul>
                  <li class="w-icon active">
                    <a href="#">
                      <i class="icon_bag_alt"></i>
                    </a>
                  </li>
                  <li class="quick-view">
                    <a href="product.html">+ Quick View</a>
                  </li>
                </ul>
              </div>
              <div class="pi-text">
                <div class="catagory-name">Tablet</div>
                <a href="#">
                  <h5>Wacom Cintiq DTC 330</h5>
                </a>
                <div class="product-price">
                  Rp 5.999.000
                  <!-- <span>$35.00</span> -->
                </div>
              </div>
            </div>
            <div class="product-item">
              <div class="pi-pic">
                <img src="images/products/rexus-gaming-chair-rgc-111-thumb.jpg" alt />
                <ul>
                  <li class="w-icon active">
                    <a href="#">
                      <i class="icon_bag_alt"></i>
                    </a>
                  </li>
                  <li class="quick-view">
                    <a href="#">+ Quick View</a>
                  </li>
                </ul>
              </div>
              <div class="pi-text">
                <div class="catagory-name">Gaming Chair</div>
                <a href="#">
                  <h5>Rexus Gaming Chair RGC 111</h5>
                </a>
                <div class="product-price">Rp 2.500.000</div>
              </div>
            </div>
            <div class="product-item">
              <div class="pi-pic">
                <img src="images/products/figure-yukina-minato-thumb.jpg" alt />
                <ul>
                  <li class="w-icon active">
                    <a href="#">
                      <i class="icon_bag_alt"></i>
                    </a>
                  </li>
                  <li class="quick-view">
                    <a href="#">+ Quick View</a>
                  </li>
                </ul>
              </div>
              <div class="pi-text">
                <div class="catagory-name">Action Figure</div>
                <a href="#">
                  <h5>Roselia BanG Dream! Girls Band Party! Minato Yukina 1/7 Scale Figure</h5>
                </a>
                <div class="product-price">Rp 2.400.000</div>
              </div>
            </div>
            <div class="product-item">
              <div class="pi-pic">
                <img src="images/products/apx-600-guitar-thumb.jpg" alt />
                <ul>
                  <li class="w-icon active">
                    <a href="#">
                      <i class="icon_bag_alt"></i>
                    </a>
                  </li>
                  <li class="quick-view">
                    <a href="#">+ Quick View</a>
                  </li>
                  <li class="w-icon">
                    <a href="#">
                      <i class="fa fa-random"></i>
                    </a>
                  </li>
                </ul>
              </div>
              <div class="pi-text">
                <div class="catagory-name">Guitar</div>
                <a href="#">
                  <h5>Gitar Yamaha Akustik Elektrik APX-600 </h5>
                </a>
                <div class="product-price">Rp 2.450.000</div>
              </div>
            </div>
            <div class="product-item">
              <div class="pi-pic">
                <img src="images/products/samsung-galaxy-note-10-plus-thumb.jpg" alt />
                <ul>
                  <li class="w-icon active">
                    <a href="#">
                      <i class="icon_bag_alt"></i>
                    </a>
                  </li>
                  <li class="quick-view">
                    <router-link to="/product">+ Quick View</router-link>
                  </li>
                  <li class="w-icon">
                    <a href="#">
                      <i class="fa fa-random"></i>
                    </a>
                  </li>
                </ul>
              </div>
              <div class="pi-text">
                <div class="catagory-name">Smartphone</div>
                <a href="#">
                  <h5>Samsung Galaxy Note10+ 256GB - Aura Black</h5>
                </a>
                <div class="product-price">Rp 16.099.000</div>
              </div>
            </div>
          </carousel>
        </div>
      </div>
    </div>
  </section>
  <!-- Women Banner Section End -->
</template>

<script>

import carousel from "vue-owl-carousel";

export default {
  name: "BannerLunaShop",
  components: {
    carousel
  }
};
</script>

<style scoped>
.product-item {
    margin-right: 25px;
}
</style>
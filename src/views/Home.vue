<template>
  <div class="home">
    <HeaderLunaShop />
    <HeroLunaShop />
    <BannerLunaShop />
    <GalleryLunaShop />
    <PartnerLunaShop />
    <FooterLunaShop />
  </div>
</template>

<script>
// @ is an alias to /src
import HeaderLunaShop from "@/components/HeaderLunaShop.vue";
import HeroLunaShop from "@/components/HeroLunaShop.vue";
import BannerLunaShop from "@/components/BannerLunaShop.vue";
import GalleryLunaShop from "@/components/GalleryLunaShop.vue";
import PartnerLunaShop from "@/components/PartnerLunaShop.vue";
import FooterLunaShop from "@/components/FooterLunaShop.vue";

export default {
  name: "Home",
  components: {
    HeaderLunaShop,
    HeroLunaShop,
    BannerLunaShop,
    GalleryLunaShop,
    PartnerLunaShop,
    FooterLunaShop
  }
};
</script>

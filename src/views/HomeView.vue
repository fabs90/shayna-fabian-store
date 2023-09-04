<template>
  <div class="home">
    <HeaderShop />
    <HeroView></HeroView>
    <WomanBanner></WomanBanner>
    <Instasection></Instasection>
    <LogoPartner></LogoPartner>
    <FooterShop />
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";
import HeaderShop from "@/components/HeaderShop.vue";
import HeroView from "@/components/Hero.vue";
import WomanBanner from "@/components/WomanBanner.vue";
import Instasection from "@/components/InstaSection.vue";
import LogoPartner from "@/components/LogoPartner.vue";
import FooterShop from "@/components/FooterShop.vue";

export default {
  name: "HomeView",
  components: {
    HeaderShop,
    HeroView,
    WomanBanner,
    Instasection,
    LogoPartner,
    FooterShop,
  },
};
</script>

<style>
.carousel__item {
  width: 100%;
  font-size: 20px;
  border-radius: 8px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.carousel__slide {
  padding: 10px;
}

.carousel__prev,
.carousel__next {
  box-sizing: content-box;
  border: 5px solid white;
}
</style>

<template>
  <!-- Partner Logo Section Begin -->

  <div class="partner-logo">
    <div class="container">
      <h3 class="mb-4 partners-text">Our Partners</h3>
      <div class="logo-carousel">
        <Carousel :autoplay="3000" :wrap-around="true" :items-to-show="3">
          <Slide v-for="slide in 1" :key="slide">
            <div class="carousel__item logo-item">
              <div class="tablecell-inner">
                <img src="img/logo-carousel/logo-1.png" alt="" />
              </div>
            </div>
          </Slide>
          <Slide v-for="slide in 1" :key="slide">
            <div class="carousel__item logo-item">
              <div class="tablecell-inner">
                <img src="img/logo-carousel/logo-2.png" alt="" />
              </div>
            </div>
          </Slide>
          <Slide v-for="slide in 1" :key="slide">
            <div class="carousel__item logo-item">
              <div class="tablecell-inner">
                <img src="img/logo-carousel/logo-3.png" alt="" />
              </div>
            </div>
          </Slide>
          <Slide v-for="slide in 1" :key="slide">
            <div class="carousel__item logo-item">
              <div class="tablecell-inner">
                <img src="img/logo-carousel/logo-4.png" alt="" />
              </div>
            </div>
          </Slide>
          <Slide v-for="slide in 1" :key="slide">
            <div class="carousel__item logo-item">
              <div class="tablecell-inner">
                <img src="img/logo-carousel/logo-5.png" alt="" />
              </div>
            </div>
          </Slide>
        </Carousel>
      </div>
    </div>
  </div>

  <!-- Partner Logo Section End -->
</template>
<script>
import { defineComponent } from "vue";
import { Carousel, Slide } from "vue3-carousel";

import "vue3-carousel/dist/carousel.css";

export default defineComponent({
  name: "LogoPartner",
  components: {
    Carousel,
    Slide,
  },
});
</script>

<style>
.partners-text {
  color: white;
  font-weight: bold;
  font-size: 2rem;
}
</style>

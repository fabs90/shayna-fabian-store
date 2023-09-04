<template>
  <!-- Hero Section Begin -->
  <section class="hero-section">
    <Carousel class="hero-items" :autoplay="2000" :wrap-around="true">
      <Slide v-for="slide in 1" :key="slide">
        <div
          class="single-hero-items set-bg carousel__item"
          style="background-image: URL('/img/hero-1.jpg')"
        >
          <div class="container">
            <div class="row">
              <div class="col-lg-5">
                <h2>Bag,kids</h2>
                <h4>
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed
                  do eiusmod tempor incididunt ut labore et dolore
                </h4>
                <a href="#" class="primary-btn">Shop Now</a>
              </div>
            </div>
          </div>
        </div>
      </Slide>
      <Slide v-for="slide in 1" :key="slide">
        <div
          class="single-hero-items set-bg carousel__item"
          style="background-image: URL('/img/hero-2.jpg')"
        >
          <div class="container">
            <div class="row">
              <div class="col-lg-5">
                <h2>Black friday</h2>
                <h4>
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed
                  do eiusmod tempor incididunt ut labore et dolore
                </h4>
                <a href="#" class="primary-btn">Shop Now</a>
              </div>
            </div>
          </div>
        </div>
      </Slide>
      <Slide v-for="slide in 1" :key="slide">
        <div
          class="single-hero-items set-bg carousel__item"
          style="background-image: URL('/img/hero-3.jpg')"
        >
          <div class="container">
            <div class="row">
              <div class="col-lg-5 ml-auto">
                <h2 class="text-right">Black friday</h2>
                <h4 class="text-right">
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed
                  do eiusmod tempor incididunt ut labore et dolore
                </h4>
                <a href="#" class="primary-btn">Shop Now</a>
              </div>
            </div>
          </div>
        </div>
      </Slide>

      <template #addons>
        <Navigation />
        <Pagination />
      </template>
    </Carousel>
  </section>
  <!-- Hero Section End -->
</template>

<script>
import { Carousel, Navigation, Pagination, Slide } from "vue3-carousel";

import "vue3-carousel/dist/carousel.css";

export default {
  name: "HeroView",
  components: {
    Carousel,
    Navigation,
    Pagination,
    Slide,
  },
};
</script>

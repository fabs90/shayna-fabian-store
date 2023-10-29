<template>
  <!-- Product Shop Section Begin -->
  <section class="product-shop spad page-details">
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div class="row">
            <div class="col-lg-6">
              <div class="product-pic-zoom">
                <img class="product-big-img" :src="product_img_main" alt="" />
              </div>
              <div class="product-thumbs">
                <Carousel
                  :autoplay="false"
                  :wrap-around="true"
                  :items-to-show="3"
                >
                  <Slide v-for="slide in 1" :key="slide">
                    <div
                      class="pt"
                      @click="changeImage(thumbs[0])"
                      :class="thumbs[0] == product_img_main ? 'active' : ''"
                    >
                      <img src="../../../public/img/mickey1.jpg" alt="" />
                    </div>
                  </Slide>
                  <Slide v-for="slide in 1" :key="slide">
                    <div
                      class="pt"
                      @click="changeImage(thumbs[1])"
                      :class="thumbs[1] == product_img_main ? 'active' : ''"
                    >
                      <img src="../../../public/img/mickey2.jpg" alt="" />
                    </div>
                  </Slide>
                  <Slide v-for="slide in 1" :key="slide">
                    <div
                      class="pt"
                      @click="changeImage(thumbs[2])"
                      :class="thumbs[2] == product_img_main ? 'active' : ''"
                    >
                      <img src="../../../public/img/mickey3.jpg" alt="" />
                    </div>
                  </Slide>
                  <Slide v-for="slide in 1" :key="slide">
                    <div
                      class="pt"
                      @click="changeImage(thumbs[3])"
                      :class="thumbs[3] == product_img_main ? 'active' : ''"
                    >
                      <img src="../../../public/img/mickey4.jpg" alt="" />
                    </div>
                  </Slide>
                </Carousel>
              </div>
            </div>
            <div class="col-lg-6 text-left">
              <div class="product-details">
                <div class="pd-title">
                  <span>oranges</span>
                  <h3>Pure Pineapple</h3>
                </div>
                <div class="pd-desc">
                  <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Corporis, error officia. Rem aperiam laborum voluptatum vel,
                    pariatur modi hic provident eum iure natus quos non a sequi,
                    id accusantium! Autem.
                  </p>
                  <p>
                    Lorem ipsum dolor sit, amet consectetur adipisicing elit.
                    Quam possimus quisquam animi, commodi, nihil voluptate
                    nostrum neque architecto illo officiis doloremque et
                    corrupti cupiditate voluptatibus error illum. Commodi
                    expedita animi nulla aspernatur. Id asperiores blanditiis,
                    omnis repudiandae iste inventore cum, quam sint molestiae
                    accusamus voluptates ex tempora illum sit perspiciatis.
                    Nostrum dolor tenetur amet, illo natus magni veniam quia sit
                    nihil dolores. Commodi ratione distinctio harum voluptatum
                    velit facilis voluptas animi non laudantium, id dolorem
                    atque perferendis enim ducimus? A exercitationem recusandae
                    aliquam quod. Itaque inventore obcaecati, unde quam impedit
                    praesentium veritatis quis beatae ea atque perferendis
                    voluptates velit architecto?
                  </p>
                  <h4>$495.00</h4>
                </div>
                <div class="quantity">
                  <router-link to="/cart"
                    ><a href="#/cart" class="primary-btn pd-cart"
                      >Add To Cart</a
                    ></router-link
                  >
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- Product Shop Section End -->
</template>

<script>
import { Carousel, Slide } from "vue3-carousel";

import "vue3-carousel/dist/carousel.css";
export default {
  name: "ProductSectionView",
  components: {
    Carousel,
    Slide,
  },
  data() {
    return {
      product_img_main: "img/mickey1.jpg",
      thumbs: [
        "img/mickey1.jpg",
        "img/mickey2.jpg",
        "img/mickey3.jpg",
        "img/mickey4.jpg",
      ],
    };
  },
  methods: {
    changeImage(urlImage) {
      this.product_img_main = urlImage;
    },
  },
};
</script>

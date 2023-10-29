<template>
  <div class="product">
    <HeaderShop></HeaderShop>
    <BreacrumpView />
    <ProductSectionViewVue></ProductSectionViewVue>
    <RelatedProductView />
    <FooterShop></FooterShop>
  </div>
</template>

<script>
import HeaderShop from "@/components/HeaderShop.vue";
import BreacrumpView from "@/components/product/BreacrumbView.vue";
import ProductSectionViewVue from "@/components/product/ProductSectionView.vue";
import RelatedProductView from "@/components/product/RelatedProductView.vue";
import FooterShop from "@/components/FooterShop.vue";

export default {
  name: "ProductView",
  components: {
    HeaderShop,
    BreacrumpView,
    ProductSectionViewVue,
    RelatedProductView,
    FooterShop,
  },
};
</script>

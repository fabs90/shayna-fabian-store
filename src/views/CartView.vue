<template>
  <HeaderShop></HeaderShop>
  <BreacrumpView></BreacrumpView>
  <CartSectionVue />
  <FooterShop></FooterShop>
</template>
<script>
import HeaderShop from "@/components/HeaderShop.vue";
import FooterShop from "@/components/FooterShop.vue";
import BreacrumpView from "@/components/product/BreacrumbView.vue";
import CartSectionVue from "@/components/card/CartSection.vue";
export default {
  name: "CartView",
  components: {
    HeaderShop,
    FooterShop,
    BreacrumpView,
    CartSectionVue,
  },
};
</script>

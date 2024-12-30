<template>
  <div class="dizme_tm_all_wrap" data-magic-cursor="show">
    <MobileHeaderVue />
    <HeaderVue />
    <HomeComponent />
    <PortfolioComponent />
    <ScrollTopVue />
  </div>
</template>

<script>
import HeaderVue from "@/components/layout/Header.vue";
import MobileHeaderVue from "@/components/layout/MobileHeader.vue";
import ScrollTopVue from "@/components/layout/ScrollTop.vue";
import HomeComponent from "../components/HomeComponent.vue";
import PortfolioComponent from "../components/PortfolioComponent.vue";

export default {
  name: "IndexView",
  components: {
    HomeComponent,
    PortfolioComponent,
    HeaderVue,
    MobileHeaderVue,
    ScrollTopVue,
  },
  // mounted() {
  //   window.addEventListener("scroll", activeSkillProgress);
  // },
};
</script>

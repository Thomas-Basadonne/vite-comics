<script>
import AppHeader from "./components/AppHeader.vue";
import ProductList from "./components/ProductList.vue";
import AppFooter from "./components/AppFooter.vue";
import BonusComponent from "./components/BonusComponent.vue";
export default {
  data() {
    return {
      title: "Main",
    };
  },
  components: {
    AppHeader,
    ProductList,
    AppFooter,
    BonusComponent,
  },
};
</script>
<template>
  <AppHeader />
  <main>
    <ProductList />
  </main>
  <BonusComponent />
  <AppFooter />
</template>
<style lang="scss">
@use "./assets/scss/general.scss";
</style>

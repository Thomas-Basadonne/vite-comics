<script>
export default {
  data() {
    return {
      title: "BonusComponent",
    };
  },
};
</script>
<template>
  <section>
    <ul class="container">
      <li class="iconCol">
        <img src="../assets/img/buy-comics-digital-comics.png" alt="img" />
        DIGITAL COMICS
      </li>
      <li class="iconCol">
        <img src="../assets/img/buy-comics-merchandise.png" alt="img" /> DC
        MERCHANDISE
      </li>
      <li class="iconCol">
        <img src="../assets/img/buy-comics-subscriptions.png" alt="img" />
        SUBSCRIPTION
      </li>
      <li class="iconCol">
        <img src="../assets/img/buy-comics-shop-locator.png" alt="img" />
        COMIC SHOP LOCATOR
      </li>
      <li class="iconCol">
        <img src="../assets/img/buy-dc-power-visa.svg" alt="img" /> DC POWER
        VISA
      </li>
    </ul>
  </section>
</template>
<style lang="scss" scoped>
section {
  background-color: #0282f9;
  color: white;
  .container {
    display: flex;
    justify-content: space-between;
    .iconCol {
      width: 15%;
      padding: 3rem 0;
      display: flex;
      align-items: center;
      img {
        width: 50px;
        margin-right: 20px;
      }
    }
  }
}
</style>

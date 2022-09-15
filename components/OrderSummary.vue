<template>
  <section class="order">
    <div class="order-upper"></div>

    <div class="order-body">
      <p class="order-heading">Order Summary</p>
      <p class="order-info">You can now listen to millions of songs, <br/> audiobooks, and podcasts on any device <br/> anywhere you like!</p>
   
    <div class="order-plan">
      <div class="order-plan__left">
        <img class="order-icon" src="/icon-music.svg" alt="">

        <div class="order-plan__left-info">
          <p class="order-annual">Annual Plan</p>
          <p class="order-price">$59.99/year</p>
        </div>
      </div>
      <a class="order-change" href="#">Change</a>
    </div>

    <button class="order-cta">Proceed to Payment</button>

      <p class="order-cancel">Cancel Order</p>
    </div>


  </section>
</template>

<script>
export default {
  name: 'OrderSummary'
}
</script>

<style lang="scss" scoped>
@import '~/assets/_color-palette.scss';
@import '~/assets/_abstract.scss';

.order {
  width: 450px;
  height: 700px;
  background-color: colorPaletteSetting(core-white);
  border-radius: 20px;
  overflow: hidden;

  &-upper {
    height: 220px;
    background-image: url('/illustration-hero.svg');
  }

  &-body {
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    flex-direction: column;
    height: 420px;
  }

  &-heading {
    font-size: 24px;
    font-weight: 700;
  }

  &-info {
    text-align: center;
    font-size: 16px;
    color: rgb(195, 195, 195);
  }

  &-plan {
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 350px;
    height: 90px;
    background-color: #F8F9FE;
    border-radius: 20px;
  }

  &-plan__left {
    display: flex;
    width: 50%;
    justify-content: space-evenly;
    align-items: center;
  }

  &-icon {
    width: 45px;
    height: 45px;
  }

  &-annual {
    margin: 0;
    padding: 0;
    font-size: 13px;
    font-weight: 700;
  }

  &-price {
    margin: 0;
    padding: 0;
    font-size: 12px;
    color: rgb(195, 195, 195);
  }

  &-change {
    color: blue;
    font-weight: 700;
    text-decoration: underline;
    font-size: 12px;
  }

  &-cta {
    height: 50px;
    width: 350px;
    background-color: #382AE1;
    cursor: pointer;
    border: none;
    color: white;
    font-size: 14px;
    font-weight: 700;
    border-radius: 10px;

    &:hover {
      transform: scale(0.9);
    }
  }

  &-cancel {
    font-size: 12px;
    color: gray;
    font-weight: 500;
  }
}
</style>
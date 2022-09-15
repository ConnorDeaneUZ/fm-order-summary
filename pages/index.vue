<template>
<section class="container">
  <order-summary />
</section>
</template>

<script>
import OrderSummary from '../components/OrderSummary.vue'

export default {
  name: 'IndexPage',

  components: {
    OrderSummary
  }
}
</script>

<style lang="scss" scoped>
@import '~/assets/_color-palette.scss';
@import '~/assets/_abstract.scss';

.container {
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  height: 110vh;
  width: 100%;
  font-family: abstractSetting(primary_font);
  background-image: url('/pattern-background-desktop.svg');
  background-repeat: no-repeat;
  background-size: contain;
  background-color: #E0E8FF;

  @media screen and (min-width: 800px ) {
    flex-direction: row;
  }
}

body {
  margin: 0 !important;
  padding: 0 !important;
  box-sizing: border-box !important;
}
</style>
<template>
  <section class="servised">
    <div class="servised-text">
      <h3 class="descr">Services</h3>
      <h2>Our top value categories for you</h2>
    </div>
    <swiper
      :slides-per-view="3"
      :space-between="300"
      :loop="true"
      @swiper="onSwiper"
      @slideChange="onSlideChange"
    >
      <swiper-slide>
        <div class="item">
          <img src="../assets/img/destination-1.png" alt="" />
          <h5>Best Tour Guide</h5>
          <p>
            What looked like a small patch of purple grass, above five feet.
          </p>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="item">
          <img src="../assets/img/booking-1.png" alt="" />
          <h5>Easy Booking</h5>
          <p>Square, was moving across the sand in their direction.</p>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="item">
          <img
            src="../assets/img/b60e2723cae3d209928c2337a1961b6f.png"
            alt=""
          />
          <h5>Weather Forecast</h5>
          <p>
            What looked like a small patch of purple grass, above five feet.
          </p>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="item">
          <img src="../assets/img/booking-1.png" alt="" />
          <h5>Best Tour Guide</h5>
          <p>
            What looked like a small patch of purple grass, above five feet.
          </p>
        </div>
      </swiper-slide>
    </swiper>
  </section>
</template>

<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";
// Import Swiper styles
import "swiper/css";
export default {
  name: "Servised",
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    const onSwiper = (swiper) => {
      console.log(swiper);
    };
    const onSlideChange = () => {
      console.log("slide change");
    };
    return {
      onSwiper,
      onSlideChange,
    };
  },
};
</script>

<style lang="sass" scoped>
.servised
    display: flex
    align-items: center
    .servised-text
        color: #191825
        font-size: 44px
        font-style: normal
        font-weight: 700
        width: 800px
        margin-left: 8%
        h2
            font-size: 44px
            font-style: normal
            font-weight: 700
    .item
        border-radius: 32px
        background: #FFF
        text-align: center
        min-height: 445px
        width: 350px
        margin-bottom: 65px
        box-shadow: 0px 0px 0px 0px rgba(0, 0, 0, 0.10), 0px 41px 89px 0px rgba(0, 0, 0, 0.10)
        img
            width: 64px
            margin-bottom: 64px
            padding-top: 64px
        h5
            margin-bottom: 32px
            font-size: 28px
        p
            padding: 0 64px
.swiper-wrapper
    width: 500px
.swiper-slide .swiper-slide-active
    width: 500px !important
</style>

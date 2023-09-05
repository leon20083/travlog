<template>
  <section class="services">
    <div class="title">
      <h3 class="descr">Services</h3>
      <h2>Our top value categories for you</h2>
    </div>
    <Carousel
      :itemsToShow="2.35"
      :wrapAround="true"
      :snapAlign="left"
      :transition="500"
    >
      <Slide v-for="slide in itemsSlide" :key="slide">
        <div class="carousel__item">
          <img :src="slide.img" alt="" />
          <h5>{{ slide.title }}</h5>
          <p>{{ slide.text }}</p>
        </div>
      </Slide>

      ...
      <template #addons>
        <navigation />
      </template>
    </Carousel>
  </section>
</template>

<script>
import { defineComponent } from "vue";
import { Carousel, Slide, Navigation } from "vue3-carousel";

import "vue3-carousel/dist/carousel.css";

export default defineComponent({
  name: "SectionServices",
  components: {
    Carousel,
    Slide,
    Navigation,
  },
  data() {
    return {
      itemsSlide: [
        {
          img: require("../assets/img/destination-1.png"),
          title: "Best Tour Guide",
          text: "What looked like a small patch of purple grass, above five feet.",
        },
        {
          img: require("../assets/img/booking-1.png"),
          title: "Easy Booking",
          text: "Square, was moving across the sand in their direction.",
        },
        {
          img: require("../assets/img/b60e2723cae3d209928c2337a1961b6f.png"),
          title: "Weather Forecast",
          text: "What looked like a small patch of purple grass, above five feet.",
        },
      ],
    };
  },
});
</script>

<style lang="sass" scoped>
.services
  display: flex
  .title
    width: 30%
    margin-left: 5%
.carousel
  width: 70% !important
  //margin-right: -90px
.carousel__item
  // display: flex
  width: 350px
  padding: 64px
  // flex-direction: column
  // align-items: center
  //gap: 64px
  // align-self: stretch
  margin: 0
  border-radius: 32px
  background: #FFF
  img
    width: 64px
    height: 64px
    margin-bottom: 64px
  h5
    color: #191825
    text-align: center
    font-family: Circular Std
    font-size: 28px
    font-style: normal
    font-weight: 700
    margin-bottom: 32px
.carousel__slide--visible .carousel__slide--active
  box-shadow: 0px 0px 0px 0px rgba(0, 0, 0, 0.10), 0px 41px 89px 0px rgba(0, 0, 0, 0.10)
.carousel

// .carousel__slide
//   padding: 5px


.carousel__viewport
  perspective: 2000px


.carousel__track
  transform-style: preserve-3d


.carousel__slide--sliding
  transition: 0.5s


// .carousel__slide
//   opacity: 0.9
//   transform: rotateY(-20deg) scale(0.9)


// .carousel__slide--active ~ .carousel__slide
//   transform: rotateY(20deg) scale(0.9)


// .carousel__slide--prev
//   opacity: 1
//   transform: rotateY(-10deg) scale(0.95)
//   height: 445px


// .carousel__slide--next
//   opacity: 1
//   transform: rotateY(10deg) scale(0.95)
//   height: 445px


// .carousel__slide--active
//   opacity: 1
//   transform: rotateY(0) scale(1.1)
//
</style>

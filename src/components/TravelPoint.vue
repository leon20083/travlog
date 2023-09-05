<template>
  <section class="travel-point">
    <div class="tiket-star">
      <img src="../assets/img/ticket-star-1.png" alt="" />
    </div>
    <div class="price">
      <img src="../assets/img/discount-1.png" alt="" />
      <p>Discounted Price</p>
    </div>
    <img src="../assets/img/img-point.png" alt="" />
    <div class="item">
      <Title
        descr="Travel Point"
        title="We helping you find your dream location"
      />
      <p>
        Contrary to popular belief, Lorem Ipsum is not simply random text. It
        has roots in a piece of classical Latin literature from 45 BC.
      </p>
      <div class="advantages">
        <div v-for="(adv, index) in advantages" :key="index" class="item">
          <span>{{ adv.num }}</span>
          <p>{{ adv.text }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Title from "./Title.vue";
export default {
  name: "TravelPoint",
  components: {
    Title,
  },
  data() {
    return {
      advantages: [
        {
          num: "500+",
          text: "Holiday Package",
        },
        {
          num: "100",
          text: "Luxury Hotel",
        },
        {
          num: "7",
          text: "Premium Airlines",
        },
        {
          num: "2k+",
          text: "Happy Customer",
        },
      ],
    };
  },
};
</script>

<style lang="sass" scoped>
.travel-point
    position: relative
    display: flex
    padding-bottom: 143px
    .tiket-star
        position: absolute
        right: 12%
        top: 40%
        width: 64px
        height: 64px
        border-radius: 10em
        background: #FACD49
        display: flex
        justify-content: center
        align-items: center
        img
            width: 48p
    .price
        position: absolute
        left: 35%
        top: 130px
        display: flex
        align-items: center
        padding: 16px 32px
        border-radius: 100px
        background: #FFF
        box-shadow: 0px 0px 0px 0px rgba(0, 0, 0, 0.03), 0px 15px 34px 0px rgba(0, 0, 0, 0.03), 0px 62px 62px 0px rgba(0, 0, 0, 0.02), 0px 139px 83px 0px rgba(0, 0, 0, 0.01), 0px 246px 99px 0px rgba(0, 0, 0, 0.00), 0px 385px 108px 0px rgba(0, 0, 0, 0.00)
        p
            color: #191825
            font-family: Circular Std
            font-size: 23px
            font-style: normal
            font-weight: 700
            margin: 0
        img
            width: 40px
    img
        width: 55%
    .item
        width: 35%
        .title
            width: 80%
        h3
            padding-bottom: 20px
        h2, p
            width: 80%
        h2
            padding-bottom: 32px
        p
            margin-bottom: 64px
    .advantages
        display: flex
        flex-wrap: wrap
        .item
            border-radius: 32px
            border: 1px solid rgba(25, 24, 37, 0.10)
            background: #FFF
            width: 205px
            height: 150px
            margin-bottom: 32px
            text-align: center
            display: flex
            flex-direction: column
            align-items: center
            &:not(:last-child)
                margin-right: 25px

            span
                color: #FF5722
                font-family: Circular Std
                font-size: 35px
                padding: 32px 0 16px
                font-weight: 700
            p
                margin: 0 auto
</style>

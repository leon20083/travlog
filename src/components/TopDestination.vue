<template>
  <section class="top-destination">
    <img src="../assets/img/OBJECTS2.png" alt="" class="img-right" />
    <div class="container">
      <div class="title">
        <h3 class="descr">Top Destination</h3>
        <h2>Explore top destination</h2>
      </div>
      <div class="row">
        <div v-for="(item, index) in items" :key="index" class="dest-item">
          <img :src="item.img" alt="" />
          <div class="item-text">
            <div class="item-top">
              <h5>{{ item.title }}</h5>
              <span>{{ item.price }}</span>
            </div>
            <p>{{ item.text }}</p>
            <div class="reiting">
              {{ item.reiting.num }}
              <img :src="item.reiting.img" alt="" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "TopDestination",
  data() {
    return {
      items: [
        {
          img: require("../assets/img/dest-item-1.png"),
          title: "Paradise Beach, Bantayan Island",
          price: "$550.16",
          text: "Rome, Italy",
          reiting: {
            num: "4.8",
            img: require("../assets/img/star.png"),
          },
        },
        {
          img: require("../assets/img/dest-item-2.png"),
          title: "Ocean with full of Colors",
          price: "$550.16",
          text: "Maldives",
          reiting: {
            num: "4.5",
            img: require("../assets/img/star.png"),
          },
        },
        {
          img: require("../assets/img/dest-item-3.png"),
          title: "Mountain View, Above the cloud",
          price: "$550.16",
          text: "United Arab Emeries ",
          reiting: {
            num: "5.0",
            img: require("../assets/img/star.png"),
          },
        },
      ],
    };
  },
};
</script>

<style lang="sass" scoped>
.top-destination
  position: relative
  padding-bottom: 130px
  .img-right
    position: absolute
    top: 50px
    right: 0
    width: 107px
  .dest-item
    text-align: center
    width: 350px
    border-radius: 0px 0px 32px 32px
    background: #FFF
    box-shadow: 0px 0px 0px 0px rgba(0, 0, 0, 0.05), 0px 32px 71px 0px rgba(0, 0, 0, 0.05), 0px 128px 128px 0px rgba(0, 0, 0, 0.04), 0px 288px 173px 0px rgba(0, 0, 0, 0.03), 0px 513px 205px 0px rgba(0, 0, 0, 0.01), 0px 801px 224px 0px rgba(0, 0, 0, 0.00)
    img
      //width: 350px
    .item-text
      padding: 32px
      text-align: left
      .item-top
        display: flex
        justify-content: space-between
        width: 100%
        h5
          font-size: 23px
          width: 60%
        span
          color: #F85E9F
          font-family: Circular Std
          font-size: 23px
          font-style: normal
          font-weight: 700
      .reiting
        display: flex
        align-items: flex-start
        color: #FF5722
        font-family: Circular Std
        font-size: 23px
        font-style: normal
        font-weight: 700
        img
          width: 24px
          height: 24px
          margin-left: 10px
  .title
    margin-bottom: 65px
</style>

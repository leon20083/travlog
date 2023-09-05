<template>
  <section class="key-features">
    <div class="container">
      <div class="row">
        <div class="right">
          <Title descr="Key features" title="We offer best services" />
          <div class="right-text">
            <p>
              Contrary to popular belief, Lorem Ipsum is not simply random text.
              It has roots in a piece of classical Latin literature from 45 BC.
            </p>
          </div>
        </div>
        <div class="left">
          <img class="img-1" src="../assets/img/img-features-1.png" alt="" />
          <img class="img-2" src="../assets/img/img-features-2.png" alt="" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Title from "./Title.vue";
export default {
  name: "KeyFeatures",
  components: {
    Title,
  },
};
</script>

<style lang="sass" scoped>
.key-features
    .right
        width: 50%
        .title
            padding-bottom: 32px
    .left
        position: relative
        width: 50%
        .img-1
            width: 443px
            padding-bottom: 107px
        .img-2
            position: absolute
            bottom: 0
            right: 0
            width: 375px
</style>

<template>
  <div class="companions">
    <div class="container">
      <div class="row">
        <div class="item">
          <img src="../assets/img/item-1.png" alt="" />
        </div>
        <div class="item">
          <img src="../assets/img/item-2.png" alt="" />
        </div>
        <div class="item">
          <img src="../assets/img/item-3.png" alt="" />
        </div>
        <div class="item">
          <img src="../assets/img/item-4.png" alt="" />
        </div>
        <div class="item">
          <img src="../assets/img/item-5.png" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Companions",
};
</script>

<style lang="sass" scoped>
.companions
    position: relative
    padding-bottom: 50px
    .img-left
        position: absolute
        left: 40px
    .item
        padding: 65px 50px
        margin-top: 50px
</style>

<template>
  <div class="menu">
    <ul>
      <li><a href="/" class="active">Home</a></li>
      <li><a href="#discover">Discover</a></li>
      <li><a href="#specialDeals">Special Deals</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Menu",
};
</script>

<style lang="sass" scoped>
.menu
    width: 55%
    ul
        display: flex
        justify-content: space-around
        padding: 0
        li
            list-style: none
            a
                text-decoration: none
                color: rgba(25, 24, 37, 0.50)
                font-family: Circular Std
                font-size: 14px
                font-style: normal
                font-weight: 700
                &.active
                    color: #222831
</style>

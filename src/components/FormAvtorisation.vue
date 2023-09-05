<template>
  <form class="form">
    <input type="text" placeholder="Login" />
    <button type="submit" class="btn">Sign Up</button>
  </form>
</template>

<script>
export default {
  name: "FormAvtorisation",
};
</script>

<style lang="sass" scoped>
.form
  display: flex
  width: 25%
  input
    border: none
    width: 115px
    outline: none
    &::placeholder
      padding: 16px 32px
      color: #222831 !important
      font-family: Circular Std
      font-size: 14px
      font-style: normal
      font-weight: 700
</style>

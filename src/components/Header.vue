<template>
  <header class="header">
    <div class="container">
      <div class="row">
        <Logo />
        <Menu />
        <FormAvtorisation />
      </div>
    </div>
  </header>
</template>

<script>
import Logo from "./Logo.vue";
import Menu from "./Menu.vue";
import FormAvtorisation from "./FormAvtorisation.vue";
export default {
  name: "Header",
  components: {
    Logo,
    Menu,
    FormAvtorisation,
  },
};
</script>

<style lang="sass" scoped>
.header
    padding: 32px 0
    margin-bottom: 64px
</style>

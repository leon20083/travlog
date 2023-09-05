<template>
  <div class="item-text">
    <h2>{{ text }}</h2>
    <img src="" alt="" />
  </div>
</template>

<script>
export default {
  name: "SectionItem",
  props: {
    text: {
      type: String,
      required: true,
    },
  },
};
</script>

<style lang="sass" scoped></style>

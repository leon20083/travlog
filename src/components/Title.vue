<template>
  <div class="title">
    <h3 class="descr">{{ descr }}</h3>
    <h2>{{ title }}</h2>
  </div>
</template>

<script>
export default {
  name: "Title",
  props: {
    descr: {
      type: String,
      required: true,
    },
    title: {
      type: String,
      required: true,
    },
  },
};
</script>

<style lang="sass" scoped></style>

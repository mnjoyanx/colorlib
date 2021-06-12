<template>
  <header id="header">
    <m-navbar />
    <m-header-slider />
  </header>
</template>

<script>
export default {
  name: "Header",
  components: {
    MNavbar: () => import("./Navbar"),
    MHeaderSlider: () => import("./HeaderSlider.vue"),
  },
};
</script>

<style lang="scss" scoped></style>

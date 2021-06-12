<template>
  <div id="app">
    <m-header />
    <m-about />
  </div>
</template>

<script>
export default {
  name: "App",
  components: {
    MHeader: () => import("@/components/Header"),
    MAbout: () => import("@/components/About"),
  },
};
</script>

<style lang="scss">
@import "/public/stylesheets/app";
</style>

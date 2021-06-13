<template>
  <div id="app">
    <m-header />
    <m-about />
    <m-results />
  </div>
</template>

<script>
export default {
  name: "App",
  components: {
    MHeader: () => import("@/components/Header"),
    MAbout: () => import("@/components/About"),
    MResults: () => import("@/components/Results"),
  },
};
</script>

<style lang="scss">
@import "/public/stylesheets/app";
</style>

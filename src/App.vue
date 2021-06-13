<template>
  <div id="app">
    <m-header />
    <m-about />
    <m-results />
    <m-work-flow />
    <m-services />
    <m-projects />
    <m-design />
    <m-testimony />
  </div>
</template>

<script>
export default {
  name: "App",
  components: {
    MHeader: () => import("@/components/Header"),
    MAbout: () => import("@/components/About"),
    MResults: () => import("@/components/Results"),
    MWorkFlow: () => import("@/components/WorkFlow"),
    MServices: () => import("@/components/Services"),
    MProjects: () => import("@/components/Projects"),
    MDesign: () => import("@/components/Design"),
    MTestimony: () => import("@/components/Testimony"),
  },
};
</script>

<style lang="scss">
@import "/public/stylesheets/app";
</style>

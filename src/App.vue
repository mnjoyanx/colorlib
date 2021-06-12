<template>
  <div id="app">
    <m-header />
  </div>
</template>

<script>
export default {
  name: "App",
  components: {
    MHeader: () => import("@/components/MHeader"),
  },
};
</script>

<style lang="scss"></style>

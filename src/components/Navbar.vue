<template>
  <nav id="navbar">
    <div class="container">
      <div class="navbar--main">
        <h1 class="navbar--main_title">
          <a href="#">Mosaic</a>
        </h1>
        <ul class="navbar--main_menu">
          <li><a href="#" class="active">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Project</a></li>
          <li><a href="#">Services</a></li>
          <li><a href="#">Team</a></li>
          <li><a href="#">Blog</a></li>
          <li><a href="#">Contact</a></li>
        </ul>
        <div class="menu--controller" @click="openMenu">
          <span
            class="iconify"
            data-icon="ant-design:menu-outlined"
            data-inline="false"
          ></span>
          <p class="open--menu_text">Menu</p>
        </div>
      </div>
      <ul class="navbar--main_tablet" :class="{ 'opened-menu': isOpen }">
        <li><a href="#" class="active">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Project</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">Team</a></li>
        <li><a href="#">Blog</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
  data() {
    return {
      isOpen: false,
    };
  },
  methods: {
    openMenu() {
      this.isOpen = !this.isOpen;
    },
  },
};
</script>

<style lang="scss" scoped>
@import "public/stylesheets/components/navbar";
</style>

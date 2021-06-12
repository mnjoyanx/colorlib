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
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style lang="scss" scoped>
@import "public/stylesheets/components/navbar";
</style>

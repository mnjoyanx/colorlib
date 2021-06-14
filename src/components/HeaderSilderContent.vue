<template>
  <div>
    <div class="container slider-container">
      <div class="slider--bg" :class="bgImg">
        <div class="slider--main_content">
          <h2
            class="slider--main_content_title"
            v-for="item in title"
            :key="item"
          >
            {{ item }}
          </h2>
          <div class="slider--main_content_content">
            <p class="slider--main_content_text">
              {{ text }}
            </p>
          </div>
          <button class="slider--main_content_btn">view our works</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MHeaderSliderContent",
  props: {
    title: {
      type: Array,
      required: true,
    },
    text: {
      type: String,
      required: true,
    },

    sticky: {
      type: String,
      default: () => "",
    },

    bgImg: {
      type: String,
      required: true,
    },
  },
};
</script>

<style lang="scss" scoped>
@import "/public/stylesheets/components/headerSlider";
</style>

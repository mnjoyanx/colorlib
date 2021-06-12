<template>
  <div class="header--slider_main">
    <swiper :auto-update="true" ref="mySwiper" :options="options">
      <swiper-slide v-for="item in slider" :key="item.id">
        <m-header-slider-content
          :title="item.title"
          :text="item.text"
          :sticky="item.sticky"
          :bg-img="item.bgImg"
        />
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
import { Swiper, SwiperSlide, directive } from "vue-awesome-swiper";

import "swiper/css/swiper.css";

export default {
  name: "MHeaderSlider",
  components: {
    Swiper,
    SwiperSlide,
    MHeaderSliderContent: () => import("./HeaderSilderContent"),
  },
  computed: {
    swiper() {
      return this.$refs.mySwiper.$swiper;
    },
  },
  directives: {
    swiper: directive,
  },
  data() {
    return {
      slider: [
        {
          title: ["We Love", "Modern Designs"],
          text: [
            "A small river named Duden flows by their place and supplies it with the",
            "necessary regelialia. It is a paradisematic country, in which roasted",
            "parts of sentences fly into your mouth.",
          ],
          sticky: "ARCHITECTURE FIRM",
          bgImg: "amazing",
        },
        {
          title: ["We Create Amazing", "Architecture", "Designs"],
          text: [
            "A small river named Duden flows by their place and supplies it with the",
            "necessary regelialia. It is a paradisematic country, in which roasted",
            "parts of sentences fly into your mouth.",
          ],
          sticky: "SINCE - 2018",
          bgImg: "modern",
        },
      ],
      options: {
        autoplay: true,
        // effect: "zoom",
        loop: true,
        navigation: {
          nextEl: ".swiper-button-next",
          prevEl: ".swiper-button-prev",
        },
      },
    };
  },
  methods: {
    onSwiper(swiper) {
      console.log(swiper, 555);
    },
    onSlideChange() {
      console.log("slide change");
    },
  },
};
</script>

<style lang="scss" scoped>
.header--slider_main {
  height: 100vh;
}
</style>

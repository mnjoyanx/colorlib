<template>
  <section id="testimony">
    <div class="container">
      <div class="testimony--main_header">
        <div class="testimony--main_header_first">
          <p>TESTIMONY</p>
          <span></span>
        </div>
        <p class="testimony--main_header_customer">
          Our satisfied customer says
        </p>
        <p class="testimony--main_header_country">
          Far far away, behind the word mountains, far from the countries
          Vokalia and Consonantia, there live the blind texts. Separated they
          live in
        </p>
      </div>
      <swiper ref="mySwiper" :options="swiperOptions">
        <swiper-slide v-for="item in customers" :key="item.id">
          <div class="slider-main">
            <div class="slier--main__content">
              <div class="slier--main__content_img">
                <img :src="item.img" alt="" />
                <span>
                  <font-awesome-icon icon="user-secret" class="user-secret" />
                </span>
              </div>
              <p>{{ item.text }}</p>
              <div>
                <p>{{ item.name }}</p>
                <p>{{ item.info }}</p>
              </div>
            </div>
          </div>
        </swiper-slide>
        <div class="swiper-pagination" slot="pagination"></div>
      </swiper>
    </div>
  </section>
</template>

<script>
import { Swiper, SwiperSlide, directive } from "vue-awesome-swiper";
import "swiper/css/swiper.css";
export default {
  name: "Testimony",
  data() {
    return {
      customers: [
        {
          id: 0,
          img: "https://preview.colorlib.com/theme/mosaic/images/xperson_3.jpg.pagespeed.ic.Cln-jaM1jK.webp",
          text: "Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.",
          name: "Garreth Smith",
          info: "Exterior Designer",
        },
        {
          id: 1,
          img: "https://preview.colorlib.com/theme/mosaic/images/xperson_1.jpg.pagespeed.ic.a2MnMHMs44.webp",
          text: "Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.",
          name: "Garreth Smith",
          info: "Exterior Designer",
        },
        {
          id: 2,
          img: "https://preview.colorlib.com/theme/mosaic/images/xperson_2.jpg.pagespeed.ic.Xrdu_nPZRp.webp",
          text: "Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.",
          name: "Garreth Smith",
          info: "Exterior Designer",
        },
        {
          id: 3,
          img: "https://preview.colorlib.com/theme/mosaic/images/xperson_3.jpg.pagespeed.ic.Cln-jaM1jK.webp",
          text: "Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.",
          name: "Garreth Smith",
          info: "Exterior Designer",
        },
        {
          id: 4,
          img: "https://preview.colorlib.com/theme/mosaic/images/xperson_1.jpg.pagespeed.ic.a2MnMHMs44.webp",
          text: "Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.",
          name: "Garreth Smith",
          info: "Exterior Designer",
        },
        {
          id: 5,
          img: "https://preview.colorlib.com/theme/mosaic/images/xperson_2.jpg.pagespeed.ic.Xrdu_nPZRp.webp",
          text: "Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.",
          name: "Garreth Smith",
          info: "Exterior Designer",
        },
      ],
      freeMode: true,

      swiperOptions: {
        slidesPerView: 3,
        spaceBetween: 0,
        loop: true,
        pagination: {
          el: ".swiper-pagination",
        },

        breakpoints: {
          1024: {
            slidesPerView: 3,
          },
          768: {
            slidesPerView: 3,
          },
          640: {
            slidesPerView: 2,
          },
          320: {
            slidesPerView: 1,
          },
        },
      },
    };
  },
  components: {
    Swiper,
    SwiperSlide,
  },
  directives: {
    swiper: directive,
  },
};
</script>

<style lang="scss" scoped>
@import "/public/stylesheets/components/testimony";
</style>

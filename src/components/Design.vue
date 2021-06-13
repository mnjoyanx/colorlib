<template>
  <section id="design">
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css"
    />
    <div class="design--main">
      <div v-for="item in items" :key="item.id" class="design-item">
        <img :src="item.bgImg" alt="" />
        <div class="after--hover">
          <div class="interior-design">
            <div class="transfrom-top">
              <p>{{ item.title }}</p>
              <h2>{{ item.text }}</h2>
            </div>
            <div class="transfrom-bottom">
              <font-awesome-icon icon="user-secret" class="user-secret" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Design",
  data() {
    return {
      items: [
        {
          id: 0,
          bgImg:
            "https://preview.colorlib.com/theme/mosaic/images/xwork-1.jpg.pagespeed.ic.43nwm6im_o.webp",
          title: "INTERIOR DESIGN",
          text: "Office Interior Design",
        },
        {
          id: 1,
          bgImg:
            "	https://preview.colorlib.com/theme/mosaic/images/xwork-2.jpg.pagespeed.ic.XI13o5XZJq.webp",
          title: "INTERIOR DESIGN",
          text: "Office Interior Design",
        },
        {
          id: 2,
          bgImg:
            "	https://preview.colorlib.com/theme/mosaic/images/xwork-3.jpg.pagespeed.ic.Rg0pRbH0-_.webp",
          title: "INTERIOR DESIGN",
          text: "Office Interior Design",
        },
        {
          id: 3,
          bgImg:
            "	https://preview.colorlib.com/theme/mosaic/images/xwork-4.jpg.pagespeed.ic.y2eTu0rfMU.webp",
          title: "INTERIOR DESIGN",
          text: "Office Interior Design",
        },
        {
          id: 4,
          bgImg:
            "https://preview.colorlib.com/theme/mosaic/images/xwork-5.jpg.pagespeed.ic.i4QQkUQ2l0.webp",
          title: "INTERIOR DESIGN",
          text: "Office Interior Design",
        },
        {
          id: 5,
          bgImg:
            "https://preview.colorlib.com/theme/mosaic/images/xwork-6.jpg.pagespeed.ic.r2t5A2RdPG.webp",
          title: "INTERIOR DESIGN",
          text: "Office Interior Design",
        },
        {
          id: 6,
          bgImg:
            "	https://preview.colorlib.com/theme/mosaic/images/xwork-7.jpg.pagespeed.ic.adHi4bUu2N.webp",
          title: "INTERIOR DESIGN",
          text: "Office Interior Design",
        },
        {
          id: 7,
          bgImg:
            "	https://preview.colorlib.com/theme/mosaic/images/xwork-8.jpg.pagespeed.ic.YAZeq70Kak.webp",
          title: "INTERIOR DESIGN",
          text: "Office Interior Design",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "/public/stylesheets/components/design";
</style>

<template>
  <section id="results">
    <div class="results--main_bg">
      <div class="results-container">
        <div class="results--main_content">
          <div
            class="results--content__main"
            v-for="(item, key) in numbers"
            :key="key"
          >
            <h2 class="results--content__main_title">{{ item.number }}</h2>
            <p class="results--content__main_text">{{ item.text }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Results",
  data() {
    return {
      numbers: [
        { number: 18, text: "Years of Experienced" },
        { number: 351, text: "Happy Clients" },
        { number: 564, text: "Finished Projects" },
        { number: 300, text: "Working Days" },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "/public/stylesheets/components/results";
</style>

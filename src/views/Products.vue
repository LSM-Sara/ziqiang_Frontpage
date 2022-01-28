<template>
  <div class="Products">
    <Header>产品</Header>
    <slideshow />
    <pageButtons
      @prev-page="prevPage"
      @next-page="nextPage"
      class="pageButtons"
    />
  </div>
</template>

<script>
// @ is an alias to /src
import Header from "../components/header.vue";
import pageButtons from "../components/pageButtons.vue";
import slideshow from "../components/slideshow.vue";
export default {
  name: "Products",
  components: {
    Header,
    pageButtons,
    slideshow,
  },
  methods: {
    prevPage() {
      this.$router.replace("/activities");
    },
    nextPage() {
      this.$router.replace("/about");
    },
  },
};
</script>
<style scoped>
.Products {
  background-image: url(../assets/background/产品首页内容@2x.png);
  background-size: cover;
  background-repeat: no-repeat;
  background-position: left top;
  overflow: hidden;
  box-sizing: border-box;
  width: 100vw;
  height: 100vh;
  background-attachment: fixed;
  position: relative;
}
.pageButtons {
  position: absolute;
  top: 75vh;
  right: 0px;
}
</style>
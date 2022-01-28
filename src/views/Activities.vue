<template>
  <div class="Activities">
    <Header>活动</Header>
    <slideshow2 />
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
import slideshow2 from "../components/slideshow2.vue";
export default {
  name: "Activities",
  components: {
    Header,
    pageButtons,
    slideshow2,
  },
  methods: {
    prevPage() {
      this.$router.replace("/");
    },
    nextPage() {
      this.$router.replace("/products");
    },
  },
};
</script>
<style scoped>
.Activities {
  background-image: url(../assets/background/活动内容@2x.png);
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
  right:0px;
}
</style>
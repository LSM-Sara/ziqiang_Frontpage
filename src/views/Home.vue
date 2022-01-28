<template>
  <div class="home-app">
    <Header>首页</Header>
    <homedisplay />
     <pageButtons
      @next-page="nextPage"
      class="pageButtons"
    />
    <decoratingButton class="decoratingButton" />
  </div>
</template>

<script>
// @ is an alias to /src
import Header from "../components/header.vue";
import decoratingButton from "../components/decoratingButton.vue";
import pageButtons from "../components/pageButtons.vue";
import Homedisplay from "../components/homedisplay.vue";
export default {
  name: "Home",
  components: {
    Header,
    pageButtons,
    Homedisplay,
    decoratingButton
  },
  methods: {
    nextPage() {
      this.$router.replace("/activities");
    },
  },
};
</script>
<style scoped>
.home-app {
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
.decoratingButton {
  position: absolute;
  top:70vh;
}
.pageButtons{
  position: absolute;
  top:75vh;
  right:0px;
}
</style>
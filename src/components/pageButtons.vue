<template>
  <div class="pageButtons-div">
    <div class="pageButton" @click="prevPage">
      <img src="../assets/icon/向上翻页.png" width="20px" />
    </div>
    <div class="pageButton" @click="toHome">
      <img src="../assets/icon/左翻页.png" width="20px" />
    </div>
    <div class="pageButton" @click="nextPage">
      <img src="../assets/icon/向下翻页.png" width="20px" />
    </div>
  </div>
</template>

<script>
export default {
  name: "pageButtons",

  methods: {
    prevPage() {
      this.$router.replace("/team");//改
    },
    toHome() {
      this.$router.replace("/home");
    },
    nextPage() {
      this.$router.replace("/team");//改
    },
  },
};
</script>
<style scoped>
.pageButtons-div{
  display: flex;
  flex-direction: column;
}
.pageButton{
  width: 32px;
  height: 32px;
  background: #e8f4fa;
  box-shadow: 2px 1px 3px 0.3px rgba(0, 0, 0, 0.1607843137254902);
  opacity: 1;
  border-radius: 50%;
  margin: 10px 0;
  text-align: center;
  
}
.pageButton:hover {
  background: #f2f9fc;
  transition: 0.3 all ease-in-out;
}
img{
  display: inline-block;
  line-height: 32px;
}
</style>
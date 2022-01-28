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
      this.$emit('prev-page');     
    },
    toHome() {
      this.$router.replace('/');
    },
    nextPage() {
      this.$emit('next-page'); 
    },
  },
};
</script>
<style scoped>
* {
  margin: 0;
  padding: 0;
}
.pageButtons-div {
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.pageButton {
  width: 40px;
  height: 40px;
  background: #e8f4fa;
  box-shadow: 2px 1px 3px 0.3px rgba(0, 0, 0, 0.1607843137254902);
  opacity: 1;
  border-radius: 50%;
  margin: 15px 20px 0px auto;
  text-align: center;
}
.pageButton:hover {
  background: #f2f9fc;
  transition: 0.3 all ease-in-out;
}
img {
  margin: 10px 0;
  display: inline-block;
}
.pageButton img:hover{
  width:18px;
}
</style>
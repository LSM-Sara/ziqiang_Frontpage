<template>
<div class="button-div">
  <div class="Button" @click="toProducts">
    <img src="../assets/icon/向下翻页.png" width="30px" />
  </div>
</div>
</template>

<script>
export default {
  name: "decoratingButton",
  methods: {
    toProducts() {
      this.$router.replace("/activities");
    },
  },
};
</script>
<style scoped>
.button-div{
  width: 100vw;
  height: 18vh;
  display: flex;
  justify-content: center;
  align-items: flex-end;
}
.Button {
  width: 45px;
  height: 45px;
  background: #f2f9fc;
  box-shadow: inset 0px 3px 6px 1px rgba(0, 0, 0, 0.1607843137254902);
  opacity: 1;
  border-radius: 50%;
  margin: 5px 5px;
  text-align: center;
}
.Button img:hover {
  margin: 15px 0;
  transition: 0.3 all ease-in-out;
}
img {
  margin: 10px 0;
  display: inline-block;
}
</style>
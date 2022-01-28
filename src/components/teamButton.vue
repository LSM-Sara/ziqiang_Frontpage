<template>
  <div class="teamButton-div">
    <div class="Button" @click="toTeam">
      <img src="../assets/icon/团队.png" width="16px" />
    </div>
    <div class="Button">
      <img src="../assets/icon/联系我们 (1).png" width="16px" />
    </div>
  </div>
</template>

<script>
export default {
  name: "teamButton",
  methods: {
    toTeam() {
      this.$router.replace("/about");
    },
  },
};
</script>
<style scoped>
.teamButton-div{
  display: flex;
}
.Button {
  width: 28px;
  height: 28px;
  background: #e8f4fa;
  box-shadow: 2px 1px 3px 0.3px rgba(0, 0, 0, 0.1607843137254902);
  opacity: 1;
  border-radius: 50%;
  margin: 5px 10px;
  text-align: center;
}
.Button:hover {
  background: #f2f9fc;
  transition: 0.3 all ease-in-out;
}
img {
  margin: 5px 0;
  display: inline-block;
}
</style>
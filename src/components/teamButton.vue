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
      this.$router.replace("/team");
    },
  },
};
</script>
<style scoped>
.Button {
  width: 20px;
  height: 20px;
  background: #e8f4fa;
  box-shadow: 2px 1px 3px 0.3px rgba(0, 0, 0, 0.1607843137254902);
  opacity: 1;
  border-radius: 50%;
}
.Button:hover {
  background: #f2f9fc;
  transition: 0.3 all ease-in-out;
}
</style>
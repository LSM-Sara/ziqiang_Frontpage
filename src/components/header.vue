<template>
  <div class="header">
    <img />
    <p>新拟态设计风格自强门户</p>
    <div></div>
    <team-button></team-button>
    <div class="teamButton" @click="toTeam">
      <img src="../assets/icon/联系我们 (1).png" width="12px" />
    </div>
  </div>
</template>
<script>
import teamButton, { teamButton } from "./teamButton.vue";

export default defineComponent({
  components: { teamButton },
  setup() {},
});
</script>

<style scoped>
.header {
  display: grid;
  width: 960px;
  height: 27px;
  background: #a1aeb4;
  box-shadow: 2.5px 1.5px 4px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  border-radius: 0px 0px 0px 0px;
  opacity: 1;
}
.header p {
  width: 88px;
  height: 11px;
  font-size: 8px;
  font-family: Yuanti SC-Regular, Yuanti SC;
  font-weight: 400;
  color: rgba(167, 161, 161, 0.7);
  line-height: 0px;
 text-shadow: 0.3px 0.8px 1.5px #e8f4fa, 0 0 0 #000, 0.3px 0.8px 1.5px #e8f4fa;
  -webkit-background-clip: text;
  background-clip: text;
}
</style>
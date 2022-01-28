<template>
  <div class="header">
    <img src="../assets/logo-ziqiang.png" width="70px" />
    <p>新拟态设计风格自强门户</p>
    <div class="guide">
      <p><slot></slot></p>
    </div>
    <team-button></team-button>
  </div>
</template>
<script>
import teamButton from "./teamButton.vue";

export default {
  name: "Header",
  components: { teamButton },
};
</script>

<style scoped>
.header {
  display: flex;
  width: 100vw;
  height: 45px;
  background: #f2f9fc;
  box-shadow: 2.5px 1.5px 4px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  border-radius: 0px 0px 0px 0px;
  opacity: 1;
  overflow: hidden;
  align-items: center;
}
.header p {
  font-size: 12px;
  font-family: Yuanti SC-Regular, Yuanti SC;
  font-weight: 400;
  color: rgba(167, 161, 161, 0.7);
  line-height: 0px;
  text-shadow: 0.3px 0.8px 1.5px #e8f4fa, 0 0 0 #000, 0.3px 0.8px 1.5px #e8f4fa;
  -webkit-background-clip: text;
  background-clip: text;
  align-self: flex-end;
  margin: auto 30vw 15px 7px;
}
.header img {
  display: inline-block;
}
.guide {
  width: 12vw;
  height: 30px;
  background: #e8f4fa;
  box-shadow: inset 0px 3px 6px 1px rgba(0, 0, 0, 0.1607843137254902);
  border-radius: 50px 50px 50px 50px;
  opacity: 1;
  filter: blur(undefinedpx);
  text-align: center;
  margin: auto 35vw 5px 0;
}
.guide p {
  margin: 15px 0;
  display: inline-block;
  font-size: 16px;
  font-family: REEJI-CHAO-RanSerifGB-Flash-Regular, REEJI-CHAO-RanSerifGB-Flash;
  font-weight: 400;
  color: #b5afaf;
  line-height: 0px;
  text-shadow: 0.2px 0.8px 1.4px #e8f4fa, 0 0 0 #000, 0.2px 0.8px 1.4px #e8f4fa;
  -webkit-background-clip: text;
  background-clip: text;
}
</style>
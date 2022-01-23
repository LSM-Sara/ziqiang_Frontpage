<template>
  <div class="introductionCard">
    <h1 class="title">{{ title }}</h1>
    <div id="decorat"></div>
    <div class="text"><slot></slot>	</div>
    <button class="join">
      <p>join</p>
    </button>
  </div>
</template>

<script>
export default {
  name: "introductionCard",
  props: {
    title:String
  }
};
</script>

<style scoped>
.introductionCard {
  position: relative;
  width: 332px;
  height: 466.5px;
  background: #e8f4fa;
  opacity: 1;
  border: 0.5px solid #e3e0e0;
  border-radius: 10px 10px 10px 10px;
}
.title {
  position: absolute;
  left: 24%;
  top: 29px;
  font-size: 32px;
  font-family: REEJI-CHAO-RanSerifGB-Flash-Regular, REEJI-CHAO-RanSerifGB-Flash;
  font-weight: 400;
  color: rgba(167, 161, 162, 0.7);
  line-height: 0px;
  text-shadow: 0.4px 1px 1.8px #e8f4fa, 0 0 0 #000, 0.4px 1px 1.8px #e8f4fa;
  -webkit-background-clip: text;
  background-clip: text;
}
#decorat {
  position: absolute;
  top: 80px;
  left: 38%;
  width: 72px;
  height: 19.5px;
  background: #f2f9fc;
  box-shadow: 0px 1.5px 4px 0.5px rgba(0, 0, 0, 0.1607843137254902),
    inset 2.5px 1.5px 4px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  border-radius: 10px 10px 10px 10px;
  opacity: 1;
}
.text {
  position: absolute;
  left:5%;
  top: 126px;
  font-size: 14px;
  font-family: REEJI-CHAO-RanSerifGB-Flash-Regular, REEJI-CHAO-RanSerifGB-Flash;
  font-weight: 400;
  color: rgba(170, 165, 166, 0.75);
  line-height: 0px;
  letter-spacing: 1px;
  text-shadow: 0.4px 1px 1.8px #e8f4fa, 0 0 0 #000, 0.4px 1px 1.8px #e8f4fa;
  -webkit-background-clip: text;
  background-clip: text;
}
.join {
  position: absolute;
  left: 268px;
  top: 421px;
  width: 52.5px;
  height: 22.5px;
  background: #e8f4fa;
  box-shadow: 2.5px 1.5px 4px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  border-radius: 11px 11px 11px 11px;
  opacity: 1;
  border: 0.5px solid #e2dfdf;
}
.join p {
  width: 26.5px;
  height: 13px;
  display: inline;
  font-size: 12px;
  font-family: REEJI-CHAO-RanSerifGB-Flash-Regular, REEJI-CHAO-RanSerifGB-Flash;
  font-weight: 400;
  color: #b5afaf;
  line-height: 0px;
  letter-spacing: 2.5px;
  text-shadow: 0.3px 0.8px 1.5px #e8f4fa, 0 0 0 #000, 0.3px 0.8px 1.5px #e8f4fa;
  -webkit-background-clip: text;
  background-clip: text;
}
</style>
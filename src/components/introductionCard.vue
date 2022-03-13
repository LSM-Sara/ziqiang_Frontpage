<template>
  <div class="introductionCard">
    <h1 class="title">{{ title }}</h1>
    <div id="decorat"></div>
    <div class="text"><slot></slot></div>
    <button class="join">
      <p>join</p>
    </button>
  </div>
</template>

<script>
export default {
  name: "introductionCard",
  props: {
    title: String,
  },
};
</script>

<style scoped>
.introductionCard {
  display: flex;
  flex-direction: column;
  width: 400px;
  height: 550px;
  background: #e8f4fa;
  opacity: 1;
  border: 1px solid #e3e0e0;
  border-radius: 20px;
  align-items: center;
  justify-content: space-evenly;
  box-shadow: 4px 3px 5px 1px rgba(0, 0, 0, 0.1607843137254902);
}
.title {
  margin: 20px 0 10px 0;
  font-size: 36px;
  font-family: REEJI-CHAO-RanSerifGB-Flash-Regular, REEJI-CHAO-RanSerifGB-Flash;
  font-weight: 400;
  color: rgba(167, 161, 162, 0.7);
  line-height: 0px;
  text-shadow: 0.4px 1px 1.8px #e8f4fa, 0 0 0 #000, 0.4px 1px 1.8px #e8f4fa;
  -webkit-background-clip: text;
  background-clip: text;
}
#decorat {
  margin: 0 0 10px 0;
  width: 80px;
  height: 20px;
  background: #f2f9fc;
  box-shadow: 0px 1.5px 4px 0.5px rgba(0, 0, 0, 0.1607843137254902),
    inset 2.5px 1.5px 4px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  border-radius: 10px 10px 10px 10px;
  opacity: 1;
}
.text {
  height: 65%;
  width: 350px;
  font-size: 16px;
  line-height: 30px;
  font-family: REEJI-CHAO-RanSerifGB-Flash-Regular, REEJI-CHAO-RanSerifGB-Flash;
  font-weight: 400;
  color: rgba(170, 165, 166, 0.75);
  letter-spacing: 1px;
  text-shadow: 0.4px 1px 1.8px #e8f4fa, 0 0 0 #000, 0.4px 1px 1.8px #e8f4fa;
  -webkit-background-clip: text;
  background-clip: text;
}
.join {
  align-self: flex-end;
  margin: 0 5%;
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
  height: 15px;
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
<template>
  <div class="IntroductionCard-button div">
    <label>
      <input type="checkbox" :checked="checked" @input="updatedHandler" />
      <div class="IntroductionCard-button">
        <p><slot /></p>
        <img v-if="selected" src="../assets/icon/长箭头.png" />
        <img v-else src="../assets/icon/长箭头 (1).png" />
      </div>
    </label>
  </div>
</template>

<script>
export default {
  name: "IntroductionCardButton",
  props: {
      checked:{
            type:Boolean,
            default:false
        },
  },
  data() {
    return {
      selected:1,
    };
  },
  methods: {
    updatedHandler(event) {
      this.selected=0;
      this.$emit('updated',event.target.checked);
    },
  },
};
</script>
<style scoped>
.IntroductionCard-button {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 508px;
  height: 64px;
  background: #e8f4fa;
  box-shadow: 2.5px 1.5px 4px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  border-radius: 19px 19px 19px 19px;
  opacity: 1;
  border: 0.5px solid #e5e5e5;
}
.IntroductionCard-button p {
  margin: 0 30px;
  font-size: 24px;
  font-family: REEJI-CHAO-RanSerifGB-Flash-Regular, REEJI-CHAO-RanSerifGB-Flash;
  font-weight: 400;
  color: rgba(181, 175, 175, 0.75);
  line-height: 0px;
  letter-spacing: 2.5px;
  text-shadow: 0.4px 1px 1.8px #e8f4fa, 0 0 0 #000, 0.4px 1px 1.8px #e8f4fa;
  -webkit-background-clip: text;
  background-clip: text;
}
img {
   margin: 0 20px;
  width: 40px;
  height: 40px;
  opacity: 1;
}
input {
  display: none;
}
input[type="checkbox"]:checked + .IntroductionCard-button {
  background: #f2f9fc;
  box-shadow: 0px 1.5px 4px 0.5px rgba(0, 0, 0, 0.1607843137254902),
    inset 2.5px 1.5px 4px 0.5px rgba(0, 0, 0, 0.1607843137254902);
    transition: .3 all ease-in-out;
}
input[type="checkbox"]:checked + .IntroductionCard-button p {
  color: rgba(218, 162, 165, 0.75);
  top:8px;
  font-size: 23px;
  text-shadow: 0.4px 1px 1.8px #f2f9fc, 0 0 0 #000, 0.4px 1px 1.8px #f2f9fc;
  transition: .3 all ease-in-out;
}
</style>

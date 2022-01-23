<template>
  <div class="IntroductionCard-button div">
    <label>
      <input type="checkbox" :checked="checked" @input=" updateHandler" />
      <div class="IntroductionCard-button">
        <p><slot /></p>
        <img :src="img" />
      </div>
    </label>
  </div>
</template>

<script>
export default {
  components: { introduction },
  name: "IntroductionCard-button",
  props: {
      checked:{
            type:Boolean,
            default:false
        },
  },
  data() {
    return {
      imgarc: ["../assets/icon/长箭头.png", "../assets/icon/长箭头 (1).png"],
      img: imgsrc[0],
    };
  },
  methods: {
    updateHandler(event) {
      this.img = imgsrc[1];
      this.$emit('update',event.target.checked);
    },
  },
};
</script>
<style scoped>
.IntroCard-button {
  position: relative;
  width: 508px;
  height: 64px;
  background: #e8f4fa;
  box-shadow: 2.5px 1.5px 4px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  border-radius: 19px 19px 19px 19px;
  opacity: 1;
  border: 0.5px solid #e5e5e5;
}
.IntroCard-button p {
  position: absolute;
  left: 31.5px;
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
  position: absolute;
  left: 451.5px;
  top: 24.5px;
  width: 30px;
  height: 15px;
  box-shadow: 2.5px 1.5px 4px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  border-radius: 0px 0px 0px 0px;
  opacity: 1;
}
input {
  display: none;
}
input[type="checkbox"]:checked + .IntroCard-button {
  background: #f2f9fc;
  box-shadow: 0px 1.5px 4px 0.5px rgba(0, 0, 0, 0.1607843137254902),
    inset 2.5px 1.5px 4px 0.5px rgba(0, 0, 0, 0.1607843137254902);
    transition: .3 all ease-in-out;
}
input[type="checkbox"]:checked + .IntroCard-button p {
  color: rgba(218, 162, 165, 0.75);
  text-shadow: 0.4px 1px 1.8px #f2f9fc, 0 0 0 #000, 0.4px 1px 1.8px #f2f9fc;
  transition: .3 all ease-in-out;
}
</style>

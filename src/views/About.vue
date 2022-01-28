<template>
  <div class="about">
    <Header id="header">团队</Header>
    <IntroductionCard :title="title[newIndex]">{{
      intro[newIndex]
    }}</IntroductionCard>
    <div class="buttons">
      <IntroductionCardButton
        :checked="checked[0]"
        @updated="(value) => updatedHandler(0, value)"
        >自强Studio</IntroductionCardButton
      >
      <IntroductionCardButton
        :checked="checked[1]"
        @updated="(value) => updatedHandler(1, value)"
        >技术中心</IntroductionCardButton
      >
      <IntroductionCardButton
        :checked="checked[2]"
        @updated="(value) => updatedHandler(2, value)"
        >新闻中心</IntroductionCardButton
      >
      <IntroductionCardButton
        :checked="checked[3]"
        @updated="(value) => updatedHandler(3, value)"
        >品牌推广中心</IntroductionCardButton
      >
      <IntroductionCardButton
        :checked="checked[4]"
        @updated="(value) => updatedHandler(4, value)"
        >站务服务中心</IntroductionCardButton
      >
      <IntroductionCardButton
        :checked="checked[5]"
        @updated="(value) => updatedHandler(5, value)"
        >运营中心</IntroductionCardButton
      >
    </div>
    <pageButtons @prev-page="prevPage" class="pageButtons" />
  </div>
</template>
<script>
import Header from "../components/header.vue";
import IntroductionCardButton from "../components/introductionButton.vue";
import IntroductionCard from "../components/introductionCard.vue";
import pageButtons from "../components/pageButtons.vue";

export default {
  name: "About",
  components: {
    Header,
    IntroductionCardButton,
    IntroductionCard,
    pageButtons,
  },
  data() {
    return {
      title: [
        "自强Studio",
        "技术中心",
        "新闻中心",
        "品牌推广中心",
        "站务服务中心",
        "运营中心",
      ],
      checked: [true, false, false, false, false, false],
      newIndex: 0,
      intro: [
        "武汉大学自强Studio，是武汉大学乃至华中地区最大的学生互联网团队之一。主要运营的线上产品包括，掌上武大微信公众号，自强网，自强学堂官方QQ、微博，自强Report、淘课啦网站、吃乎等；举办的品牌活动包括:十大珞珈风云学子评选活动、奔跑吧珞珈、毕业集市、脱机自习等。我们的愿景是成为全国最专业最有趣的高校互联网团队之一，引领武大精神。",
        "1",
        "2",
        "3",
        "4",
        "5",
      ],
    };
  },
  methods: {
    updatedHandler(index, value) {
      if (value) {
        this.newIndex = index;
      }
      let checked = [false, false, false, false, false, false];
      checked[this.newIndex] = true;
      this.checked = checked;
    },
    prevPage() {
      this.$router.replace("/products");
    },
  },
};
</script>
<style scoped>
.about {
  background-image: url(../assets/background/团队内容@2x.png);
  background-size: cover;
  background-repeat: no-repeat;
  background-position: left top;
  overflow: hidden;
  box-sizing: border-box;
  width: 100vw;
  height: 100vh;
  background-attachment: fixed;
  display: flex;
  justify-content: space-evenly;
  position: relative;
  align-items: center;
}
#header {
  position: absolute;
  left: 0px;
  top: 0px;
}
.buttons {
  display: flex;
  height: 60vh;
  flex-direction: column;
  justify-content: space-evenly;
}
.pageButtons {
  position: absolute;
  top: 75vh;
  right: 0px;
}
</style>
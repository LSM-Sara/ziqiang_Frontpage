<template>
  <div class="slideshow">
    <input type="radio" id="control-1" name="control" checked />
    <input type="radio" id="control-2" name="control" />
    <input type="radio" id="control-3" name="control" />
    <input type="radio" id="control-4" name="control" />
    <div class="controls-box">
      <div class="line"></div>
      <div class="controls-visible">
        <label for="control-1"></label>
        <label for="control-2"></label>
        <label for="control-3"></label>
        <label for="control-4"></label>
      </div>
    </div>
    <ul class="slides">
      <li class="slide">
        <div class="introduction-box">
          <div class="introduction">
            <div class="circle"></div>
            <p>
              顺着综艺“跑男”的热潮，我们推出了“奔跑吧，珞珈”系列趣味活动，从校园定向越野到大型定点户外游戏，
              “奔跑吧珞珈”系列活动已经陪我们走过了四年。春困秋乏夏打盹，不能白白辜负这万里晴空和斑斓珞珈。
              不如就突破被窝结界，解放被倦意和秋裤锁住的四肢，在秋天，来一起玩耍！
            </p>
          </div>
        </div>
        <h1>奔跑吧<span>珞珈</span></h1>
      </li>
      <li class="slide">
        <div class="introduction-box">
          <div class="introduction">
            <div class="circle"></div>
            <p>
              “十大珞珈风云学子”评选活动由党委学生工作部、党委研究生工作部、校团委、港澳台事务办公室、国际教育学院主办，
              自强Studio承办，是武汉大学最盛大的杰出学生代表评选活动之一。活动评选在道德品质、学术科研、创新创业、
              文艺体育等方面有突出表现的学生，力图展现武大人的多元风采。评审委员会由武大校长、书记、知名教师、学生评审、
              社会知名人士等共同组成，并由校长、书记亲自担任活动总顾问。
            </p>
          </div>
        </div>
        <h1>珞珈<span>风云学子</span></h1>
      </li>
      <li class="slide">
        <div class="introduction-box">
          <div class="introduction">
            <div class="circle"></div>
            <p>
              顺着综艺“跑男”的热潮，我们推出了“奔跑吧，珞珈”系列趣味活动，从校园定向越野到大型定点户外游戏，
              “奔跑吧珞珈”系列活动已经陪我们走过了四年。春困秋乏夏打盹，不能白白辜负这万里晴空和斑斓珞珈。
              不如就突破被窝结界，解放被倦意和秋裤锁住的四肢，在秋天，来一起玩耍！
            </p>
          </div>
        </div>
        <h1>奔跑吧<span>珞珈</span></h1>
      </li>
      <li class="slide">
        <div class="introduction-box">
          <div class="introduction">
            <div class="circle"></div>
            <p>
              顺着综艺“跑男”的热潮，我们推出了“奔跑吧，珞珈”系列趣味活动，从校园定向越野到大型定点户外游戏，
              “奔跑吧珞珈”系列活动已经陪我们走过了四年。春困秋乏夏打盹，不能白白辜负这万里晴空和斑斓珞珈。
              不如就突破被窝结界，解放被倦意和秋裤锁住的四肢，在秋天，来一起玩耍！
            </p>
          </div>
        </div>
        <h1>奔跑吧<span>珞珈</span></h1>
      </li>
    </ul>
  </div>
</template>


<script>
export default {
  name: "slideshow2",
};
</script>

<style scoped>
.slideshow {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
}
.controls-box {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 20px;
}
ul.slides {
  position: relative;
  width: 70vw;
  height: 500px;
  list-style: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
}
li.slide {
  margin: 0;
  padding: 0;
  width: inherit;
  height: inherit;
  position: absolute;
  top: 0;
  left: 0;
  display: flex;
  justify-content: space-around;
  align-items: center;
  transition: 0.5s transform ease-in-out;
}
.controls-visible {
  z-index: 100;
  display: flex;
  flex-direction: column;
}
.line {
  z-index: 50;
  position: absolute;
  top: -40px;
  left:7.5px;
  width: 10px;
  height: 400px;
  background: #f2f9fc;
  box-shadow: inset 2px 2px 4px 1px rgba(0, 0, 0, 0.1607843137254902);
  border-radius: 6px 6px 6px 6px;
  opacity: 1;
}
.controls-visible label {
  display: inline-block;
  width: 20px;
  height: 20px;
  background: #ebf5fa;
  box-shadow: inset 1.5px 1.5px 3px 1px rgba(0, 0, 0, 0.1607843137254902),
    2.5px 1.5px 3px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  opacity: 1;
  border: 5px solid #e8f4fa;
  border-radius: 50%;
  margin: 30px;
}
.slideshow
  input[type="radio"]:nth-of-type(1):checked
  ~ .controls-box
  .controls-visible
  label:nth-of-type(1) {
  width: 20px;
  height: 20px;
  background: #e8f4fa;
  box-shadow: 2.5px 1.5px 3px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  opacity: 1;
  border: 1px solid #eeeeee;
}

.slideshow
  input[type="radio"]:nth-of-type(2):checked
  ~ .controls-box
  .controls-visible
  label:nth-of-type(2) {
  width: 20px;
  height: 20px;
  background: #e8f4fa;
  box-shadow: 2.5px 1.5px 3px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  opacity: 1;
  border: 1px solid #eeeeee;
}

.slideshow
  input[type="radio"]:nth-of-type(3):checked
  ~ .controls-box
  .controls-visible
  label:nth-of-type(3) {
  width: 20px;
  height: 20px;
  background: #e8f4fa;
  box-shadow: 2.5px 1.5px 3px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  opacity: 1;
  border: 1px solid #eeeeee;
}

.slideshow
  input[type="radio"]:nth-of-type(4):checked
  ~ .controls-box
  .controls-visible
  label:nth-of-type(4) {
  width: 20px;
  height: 20px;
  background: #e8f4fa;
  box-shadow: 2.5px 1.5px 3px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  opacity: 1;
  border: 1px solid #eeeeee;
}
input[type="radio"] {
  display: none;
}
.slide:nth-of-type(1) {
  top: 0;
}
.slide:nth-of-type(2) {
  top: 100%;
}
.slide:nth-of-type(3) {
  top: 200%;
}
.slide:nth-of-type(4) {
  top: 300%;
}
.slideshow input[type="radio"]:nth-of-type(1):checked ~ ul.slides .slide {
  transform: translatey(0%);
}

.slideshow input[type="radio"]:nth-of-type(2):checked ~ ul.slides .slide {
  transform: translatey(-100%);
}

.slideshow input[type="radio"]:nth-of-type(3):checked ~ ul.slides .slide {
  transform: translatey(-200%);
}
.slideshow input[type="radio"]:nth-of-type(4):checked ~ ul.slides .slide {
  transform: translatey(-300%);
}
.slide h1 {
  align-self: center;
  writing-mode: vertical-rl;
  width: 100px;
  height: 100%;
  font-size: 80px;
  font-family: FZCuHeiSongS-B-GB-Regular, FZCuHeiSongS-B-GB;
  font-weight: 400;
  color: rgba(168, 163, 163, 0.7);
  text-shadow: 0.4px 1px 1.8px #e8f4fa, 0 0 0 #000, 0.4px 1px 1.8px #e8f4fa,
    1px 1px rgba(168, 163, 163, 0.05), 2px 2px rgba(168, 163, 163, 0.1),
    3px 3px rgba(168, 163, 163, 0.1), 4px 4px rgba(168, 163, 163, 0.1),
    5px 5px rgba(168, 163, 163, 0.1), 6px 6px rgba(168, 163, 163, 0.2);
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-background-clip: text;
}
.slide h1 span {
  color: rgba(212, 124, 130, 0.7);
  text-shadow: 0.4px 1px 1.8px #e8f4fa, 0 0 0 #000, 0.4px 1px 1.8px #e8f4fa,
    1px 1px rgba(212, 124, 130, 0.05), 2px 2px rgba(212, 124, 130, 0.1),
    3px 3px rgba(212, 124, 130, 0.1), 4px 4px rgba(212, 124, 130, 0.1),
    5px 5px rgba(212, 124, 130, 0.1), 6px 6px rgba(212, 124, 130, 0.2);
}
.introduction-box {
  height: 50%;
  perspective: 200px;
  -webkit-perspective: 200px;
  position: relative;
}
.introduction {
  top: 20vh;
  width: 32vw;
  border: 1px solid rgba(167, 161, 161, 0.2);
  border-radius: 10px;
  display: flex;
  justify-content: center;
  -webkit-transform: rotatey(-6deg) rotate(15deg);
  transform: rotatey(-6deg) rotate(15deg);
  background: #e8f4fa;
  box-shadow: 3px 2px 4px 1px rgba(0, 0, 0, 0.1607843137254902);
}
.introduction-box .introduction p {
  width: 28vw;
  font-size: 18px;
  font-family: REEJI-CHAO-RanSerifGB-Flash-Regular, REEJI-CHAO-RanSerifGB-Flash;
  font-weight: 400;
  color: rgba(170, 165, 166, 0.6);
  letter-spacing: 2px;
  text-shadow: 0.4px 1px 1.8px #e8f4fa, 0 0 0 #000, 0.4px 1px 1.8px #e8f4fa;
  -webkit-background-clip: text;
  background-clip: text;
  margin: 35px 20px 20px 30px;
}
.circle {
  position: absolute;
  top: 11px;
  left: 13px;
  width: 22px;
  height: 22px;
  background: #e8f4fa;
  opacity: 1;
  border: 1.2px solid #d8d8d8;
  border-radius: 11px 11px 11px 11px;
}
</style>
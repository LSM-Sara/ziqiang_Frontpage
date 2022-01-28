<template>
  <div class="displayBox">
    <div id="slogans-box1">
      <div class="slogan-box" id="first">
        <p>Learn <span>UI设计</span></p>
      </div>
      <div class="slogan-box" id="second">
        <p><span>自</span>强求是，弘毅拓<span>新</span></p>
      </div>
      <div class="slogan-box" id="third">
        <p><span>自</span>从有你，我们更<span>强</span></p>
      </div>
      <div class="slogan-box" id="forth">
        <p>热爱<span>生活</span>，热爱<span>学习</span></p>
      </div>
      <div class="slogan-box" id="fifth">
        <p>try <span>程序设计</span></p>
      </div>
    </div>
    <div class="title-box">
      <div class="title-container">
        <div class="title"><h1>自</h1></div>
        <div class="title"><h1>强</h1></div>
      </div>
      <div class="subtitle">
        <h1>studio</h1>
      </div>
      <p>-服务学生生活，记录学校发展，做有趣有品质的互联网产品-</p>
    </div>
    <div id="slogans-box2">
      <div class="slogan-box" id="refirst">
        <p>Learn UI设计</p>
      </div>
      <div class="slogan-box" id="resecond">
        <p>自强求是，弘毅拓新</p>
      </div>
      <div class="slogan-box" id="rethird">
        <p>自从有你，我们更强</p>
      </div>
      <div class="slogan-box" id="reforth">
        <p>热爱生活，热爱学习</p>
      </div>
      <div class="slogan-box" id="refifth">
        <p>try 程序设计</p>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "homedisplay",
};
</script>

<style scoped>
.displayBox {
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: 52vh;
  width: 76vw;
  position: relative;
}
#slogans-box1 {
  position: relative;
}
#slogans-box2 {
  position: relative;
  margin: 0 0 0 20vw;
}
.slogan-box {
  position: absolute;
  perspective: 200px;
  -webkit-perspective: 200px;
}
.slogan-box p {
  font-size: 30px;
  font-family: REEJI-CHAO-RanSerifGB-Flash-Regular, REEJI-CHAO-RanSerifGB-Flash;
  font-weight: 400;
  color: rgba(167, 161, 161, 0.7);
  letter-spacing: 1px;
  text-shadow: 0.4px 1px 1.8px #e8f4fa, 0 0 0 #000, 0.4px 1px 1.8px #e8f4fa;
  -webkit-background-clip: text;
  background-clip: text;
  transform: rotateY(35deg);
  -webkit-transform: rotateY(35deg);
}
.slogan-box span {
  color: rgba(231, 96, 105, 0.7);
}
#first {
  left: 155px;
  top: 0px;
  width: 190px;
  -webkit-transform: rotate(34deg);
  transform: rotate(34deg);
}
#first p {
  font-size: 25px;
}
#second {
  left: 55px;
  top: 40px;
  width: 280px;
  -webkit-transform: rotate(18deg);
  transform: rotate(18deg);
}
#third {
  top: 100px;
  width: 350px;
  -webkit-transform: rotate(5deg);
  transform: rotate(5deg);
  perspective: 200px;
  -webkit-perspective: 200px;
}
#third p {
  font-size: 35px;
}
#forth {
  left: 45px;
  top: 170px;
  width: 280px;
  -webkit-transform: rotate(-5deg);
  transform: rotate(-5deg);
}
#fifth {
  left: 155px;
  top: 230px;
  width: 160px;
  -webkit-transform: rotate(-20deg);
  transform: rotate(-20deg);
}
#fifth p {
  font-size: 25px;
}
#refirst {
  left: 15px;
  top: 0px;
  width: 190px;
  -webkit-transform: rotate(-36deg) scaleX(-1);
  transform: rotate(-36deg) scaleX(-1);
}
#refirst p {
  font-size: 25px;
}
#resecond {
  left: 16px;
  top: 40px;
  width: 280px;
  -webkit-transform: rotate(-18deg) scaleX(-1);
  transform: rotate(-18deg) scaleX(-1);
}
#rethird {
  left: 0px;
  top: 100px;
  width: 350px;
  -webkit-transform: rotate(-5deg) scaleX(-1);
  transform: rotate(-5deg) scaleX(-1);
  perspective: 200px;
  -webkit-perspective: 200px;
}
#rethird p {
  font-size: 35px;
}
#reforth {
  left: 25px;
  top: 170px;
  width: 280px;
  -webkit-transform: rotate(5deg) scaleX(-1);
  transform: rotate(5deg) scaleX(-1);
}
#refifth {
  left: 45px;
  top: 230px;
  width: 160px;
  -webkit-transform: rotate(20deg) scaleX(-1);
  transform: rotate(20deg) scaleX(-1);
}
#refifth p {
  font-size: 25px;
}
.title-box {
  position: absolute;
  display: flex;
  left: 35vw;
  top: 32vh;
  width: 30vw;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  flex-wrap: wrap;
}
.title-container {
  display: flex;
  justify-content: space-evenly;
}
.title {
  margin: 0 20px;
  width: 100px;
  height: 88px;
  background: #e8f4fa;
  box-shadow: 3px 2px 4px 0.7px rgba(0, 0, 0, 0.1607843137254902);
  border-radius: 16px 16px 16px 16px;
  opacity: 1;
  border: 0.5px solid #e8f4fa;
  text-align: center;
}
.title h1 {
  margin: auto 0;
  font-size: 60px;
  font-family: REEJI-CHAO-RanSerifGB-Flash-Regular, REEJI-CHAO-RanSerifGB-Flash;
  font-weight: 400;
  color: rgba(116, 112, 112, 0.7);
  text-shadow: 0.8px 1.5px 2px #e8f4fa, 0 0 0 #000, 0.8px 1.5px 2px #e8f4fa;
  -webkit-background-clip: text;
  background-clip: text;
}
.subtitle {
  margin: 26px 0;
  width: 250px;
  height: 45px;
  background: #e8f4fa;
  box-shadow: 3px 2px 4px 0.7px rgba(0, 0, 0, 0.1607843137254902);
  border-radius: 20px 20px 20px 20px;
  opacity: 1;
  text-align: center;
}
.subtitle h1 {
  font-size: 35px;
  font-family: Snap ITC-Regular, Snap ITC;
  font-weight: 400;
  letter-spacing: 15px;
  margin: auto 0;
  color: rgba(116, 112, 112, 0.7);
  text-shadow: 0.8px 1.5px 2px #e8f4fa, 0 0 0 #000, 0.8px 1.5px 2px #e8f4fa;
  -webkit-background-clip: text;
  background-clip: text;
}
.title-box p {
  margin: 10px 0 0 5px;
  width: 350px;
  font-size: 12px;
  font-family: FZCuHeiSongS-B-GB-Regular, FZCuHeiSongS-B-GB;
  font-weight: 400;
  color: rgba(167, 161, 161, 0.7);
  text-shadow: 0.4px 1px 1.8px #e8f4fa, 0 0 0 #000, 0.4px 1px 1.8px #e8f4fa;
  -webkit-background-clip: text;
  background-clip: text;
}
</style>
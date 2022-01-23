<template>
  <div class="slideshow">
    <ul class="slides">
      <input type="radio" id="control-1" name="control" checked />
      <input type="radio" id="control-2" name="control" />
      <input type="radio" id="control-3" name="control" />

      <li class="slide">
        <div class="app">
          <div class="circle"></div>
          <div class="download-box">
            <button><p>下载</p></button>
          </div>
        </div>
        <div class="information">
          <h1 class="title">掌上<span>武大</span></h1>
          <div class="decorat"></div>
          <p>1</p>
          <p>2</p>
          <p>3</p>
        </div>
      </li>
      <li class="slide">
        <div class="app">
          <div class="circle"></div>
          <div class="download-box">
            <button><p>下载</p></button>
          </div>
        </div>
        <div class="information">
          <h1 class="title">智慧<span>珞珈</span></h1>
          <div class="decorat"></div>
          <p>为什么是智慧珞珈</p>
          <p>这一个是简介</p>
          <p>另一个也是简介</p>
        </div>
      </li>
      <li class="slide">
        <div class="app">
          <div class="circle"></div>
          <div class="download-box">
            <button><p>下载</p></button>
          </div>
        </div>
        <div class="information">
          <h1 class="title">淘课<span>啦</span></h1>
          <div class="decorat"></div>
          <p>这里是简介</p>
          <p>还是简介</p>
          <p>另一个也是简介</p>
        </div>
      </li>
      <div class="controls-box">
        <div class="controls-visible">
          <label for="control-1"></label>
          <label for="control-2"></label>
          <label for="control-3"></label>
        </div>
      </div>
    </ul>
  </div>
</template>

<script>
export default {
  name: "slideshow",
};
</script>

<style scoped>
.slideshow {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
}

ul.slides {
  position: relative;
  width: 600px;
  height: 375px;
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
  font-family: Helvetica;
  font-size: 120px;
  transition: 0.5s transform ease-in-out;
}
.app {
  position: relative;
  width: 250px;
  height: 250px;
  margin: 0;
  padding: 0;
  background: #e8f4fa;
  box-shadow: 2.5px 2.5px 5px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  border-radius: 21px 21px 21px 21px;
  opacity: 1;
  border: 0.5px solid #e8e8e8;
  overflow: hidden;
}
.circle {
  position: absolute;
  top: 11px;
  left: 13px;
  width: 22px;
  height: 22px;
  background: #e8f4fa;
  box-shadow: 2.5px 1.5px 3px 0.5px rgba(0, 0, 0, 0.1607843137254902),
    inset 2.5px 1.5px 3px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  opacity: 1;
  border: 0.5px solid #d8d8d8;
  border-radius: 11px 11px 11px 11px;
}
.download-box {
  position: absolute;
  width: 100%;
  height: 35px;
  bottom: 0px;
  background: #f2f9fc;
  box-shadow: 0px 1.5px 3px 0.5px rgba(0, 0, 0, 0.1607843137254902),
    inset 0px 1.5px 3px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  opacity: 1;
}
.download-box button {
  position: absolute;
  bottom: 6.5px;
  right: 10.5px;
  width: 72.5px;
  height: 22px;
  background: #e8f4fa;
  box-shadow: 2.5px 1.5px 3px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  border-radius: 11px 11px 11px 11px;
  opacity: 1;
  border: 0.5px solid #f5f5f5;
}
.download-box button p {
  display: inline;
  font-size: 12px;
  font-family: REEJI-CHAO-RanSerifGB-Flash-Regular, REEJI-CHAO-RanSerifGB-Flash;
  font-weight: 400;
  color: rgba(167, 161, 161, 0.7);
  line-height: 0px;
  letter-spacing: 2.5px;
  text-shadow: 0.3px 0.8px 1.5px #e8f4fa, 0 0 0 #000, 0.3px 0.8px 1.5px #e8f4fa;
  -webkit-background-clip: text;
  background-clip: text;
}
.title {
  font-size: 60px;
  font-family: REEJI-CHAO-RanSerifGB-Flash-Regular, REEJI-CHAO-RanSerifGB-Flash;
  font-weight: 400;
  color: rgba(168, 163, 163, 0.7);
  line-height: 0px;
  text-shadow: 0.4px 1px 1.8px #e8f4fa, 0 0 0 #000, 0.4px 1px 1.8px #e8f4fa;
  -webkit-background-clip: text;
  background-clip: text;
}
.title span {
  color: rgba(212, 124, 130, 0.7);
}
.slide:nth-of-type(1) {
    left:0;
}

.slide:nth-of-type(2) {
  left: 100%;
}

.slide:nth-of-type(3) {
  left: 200%;
}

input[type="radio"] {
  position: relative;
  z-index: 100;
  display: none;
}
.decorat {
  width: 138.5px;
  height: 8px;
  background: #f2f9fc;
  box-shadow: inset 2.5px 1.5px 3px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  border-radius: 4px 4px 4px 4px;
  opacity: 1;
}
.information p {
  height: 30px;
  font-size: 15px;
  font-family: FZCuHeiSongS-B-GB-Regular, FZCuHeiSongS-B-GB;
  font-weight: 400;
  color: rgba(181, 175, 175, 0.75);
  letter-spacing: 1px;
  line-height: 0px;
  text-shadow: 0.4px 1px 1.8px #e8f4fa, 0 0 0 #000, 0.4px 1px 1.8px #e8f4fa;
  -webkit-background-clip: text;
  background-clip: text;
}
.controls-box {
  position: absolute;
  width: 100%;
  bottom: 12px;
  text-align: center;
}
.controls-visible {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 332px;
  height: 30px;
  background: #e8f4fa;
  box-shadow: 5px 3px 5px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  border-radius: 22px 22px 22px 22px;
  opacity: 1;
  border: 0.5px solid #e5e5e5;
}
.controls-visible label {
  display: inline-block;
  width: 14px;
  height: 14px;
  background-color: #f2f9fc;
  box-shadow: 0px 1.5px 2px 0.5px rgba(0, 0, 0, 0.1607843137254902),
    inset 2.5px 1.5px 2px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  opacity: 1;
  border: 0.5px solid #e5e5e5;
  border-radius: 50%;
  margin: 0 9px;
}

.slides
  input[type="radio"]:nth-of-type(1):checked
  ~ .controls-box
  .controls-visible
  label:nth-of-type(1) {
  background: #e8f4fa;
  box-shadow: 2.5px 1.5px 3px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  opacity: 1;
  border: 0.5px solid #e5e5e5;
}

.slides
  input[type="radio"]:nth-of-type(2):checked
  ~ .controls-box
  .controls-visible
  label:nth-of-type(2) {
  background: #e8f4fa;
  box-shadow: 2.5px 1.5px 3px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  opacity: 1;
  border: 0.5px solid #e5e5e5;
}

.slides
  input[type="radio"]:nth-of-type(3):checked
  ~ .controls-box
  .controls-visible
  label:nth-of-type(3) {
  background: #e8f4fa;
  box-shadow: 2.5px 1.5px 3px 0.5px rgba(0, 0, 0, 0.1607843137254902);
  opacity: 1;
  border: 0.5px solid #e5e5e5;
}

.slides input[type="radio"]:nth-of-type(1):checked ~ .slide {
  transform: translatex(0%);
}

.slides input[type="radio"]:nth-of-type(2):checked ~ .slide {
  transform: translatex(-100%);
}

.slides input[type="radio"]:nth-of-type(3):checked ~ .slide {
  transform: translatex(-200%);
}
</style>
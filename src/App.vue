<template>
  <div id="app">
    <transition name="slide-fade">
    <router-view></router-view>
    </transition>
  </div>
</template>
<script>
</script>

<style>
@font-face{
  font-family: REEJI-CHAO-RanSerifGB-Flash;
  src:url("./assets/font/潮字社国风冉宋简-闪(REEJI-CHAO-RANSERIFGB-FLASH).TTF");
}
@font-face{
  font-family: FZCuHeiSongS-B-GB;
  src:url("./assets/font/方正粗黑宋简体.TTF");
}
@font-face{
  font-family:  Snap ITC;
  src:url("./assets/font/SNAP____.TTF");
}
@font-face{
  font-family: REEJI-CHAO-YUANGBT-Flash;
  src:url("./assets/font/潮字社混元简繁-闪(REEJI-CHAO-YUANGBT-FLASH).TTF");
}
@font-face{
  font-family: REEJI-CHAO-MEIGB-FLASH-BOLD;
  src:url("./assets/font/潮字社眷美简-闪 粗体(REEJI-CHAO-MEIGB-FLASH-BOLD).TTF");
}
* {
  padding: 0;
  margin: 0;
  border: none;
  outline: none;
  box-sizing: border-box;
  scrollbar-width: none;
}

::-webkit-scrollbar {
    display: none;
}
.slide-fade-enter-active {
  transition: all .4s ease;
}
.slide-fade-leave-active {
  transition: all .4s ease;
}
.slide-fade-enter, .slide-fade-leave-to
/* .slide-fade-leave-active for below version 2.1.8 */ {
  transform: translateY(10px);
  opacity: 0;
}
</style>


<template>
  <div>
      <div class="cont">
        <div class="row">
        <div class="box top-left"><div class="cirlce"></div></div>
        <div class="box top-middle"></div>
        <div class="box top-right"></div>
      </div>
      
      <div class="row">
        <div class="box"></div>
        <div class="box middle"></div>
        <div class="box"></div>
      </div>
      <div class="row">
        <div class="box bottom-left"></div>
        <div class="box bottom-middle"></div>
        <div class="box bottom-right"></div>
      </div>
      </div>
  </div>
</template>

<script>
export default {
  name: "GameSingle"
}
</script>

<style lang="scss" scoped>
.html {
  font-size: 10px;
}
body {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
.row {
  display: flex;
}
.box {
  height: 10rem;
  width: 10rem;
  // border: 1px solid #000;
  // background-color: red;
  border: 1px solid transparent;
  cursor: pointer;
}
.cont {
  display: inline-block;
  position: relative;
  left: 50%;
  top: 50vh;
  transform: translate(-50%, -50%);
}
.top-left {
  // border-right-color: rgb(0, 4, 255);
  border-bottom-color: rgb(0, 4, 255);
}
.top-middle {
  border-right-color: rgb(0, 4, 255);
  border-left-color: rgb(0, 4, 255);
  border-bottom-color: rgb(0, 4, 255);
}
.top-right {
  border-bottom-color: rgb(0, 4, 255);
}
.middle {
  border-bottom-color: rgb(0, 4, 255);
  border-left-color: rgb(0, 4, 255);
  border-right-color: rgb(0, 4, 255);
}
.bottom-left {
  border-top-color: rgb(0, 4, 255);
}
.bottom-middle {
  border-left-color: rgb(0, 4, 255);
  border-right-color: rgb(0, 4, 255);
}
.bottom-right {
  border-top-color: rgb(0, 4, 255);
}
.d-none {
  display: none;
}
</style>
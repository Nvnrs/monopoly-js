<script setup>
import Logo from "@/components/Logo.vue";
import Row from "./Row.vue";
</script>
<template>
  <div class="board">
    <div class="board-logo">
      <Logo></Logo>
    </div>
    <div class="wrapper-rows">
      <Row position="top">
        <div class="card"></div>
        <div class="card"></div>
        <div class="card"></div>
        <div class="card"></div>
        <div class="card"></div>
        <div class="card"></div>
        <div class="card"></div>
        <div class="card"></div>
      </Row>
      <Row position="left"> </Row>
      <Row position="right"></Row>
      <Row position="bottom"></Row>
    </div>
  </div>
</template>

<style lang="scss">
.board {
  border: solid 8px black;
  width: auto;
  height: 90%;
  aspect-ratio: 1/1;
  border-radius: 1rem;
  background-color: #cde7ce;
  position: relative;
}

.board-logo {
  position: absolute;
  top: 45%;
  left: 0;
  right: 2%;
  margin: auto;
  transform: translate(-50%, -50%);
  transform: rotate(-20deg);
  pointer-events: none;
  .logo {
    height: 70px;
  }
}

.wrapper-rows {
  width: 100%;
  height: 100%;
  position: relative;
}

.card {
  border: solid 1px black;
  height: 100%;
  flex: 1;
}
</style>

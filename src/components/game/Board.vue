<script setup>
import Logo from "@/components/Logo.vue";
</script>
<template>
  <div class="board">
    <div class="board-logo">
      <Logo></Logo>
    </div>
  </div>
</template>

<style lang="scss">
.board {
  border: solid 10px black;
  height: 90%;
  width: auto;
  aspect-ratio: 1/1;
  border-radius: 1rem;
  background-color: #cde7ce;
  position: relative;
}

.board-logo {
  position: absolute;
  top: 40%;
  left: 0;
  right: 2%;
  margin: auto;
  transform: translate(-50%, -50%);
  transform: rotate(-20deg);
  .logo {
    height: 100px;
  }
}
</style>

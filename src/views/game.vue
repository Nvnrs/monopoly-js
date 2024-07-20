<script setup>
import Board from "@/components/game/Board.vue";
</script>
<template>
  <div class="game">
    <Board></Board>
  </div>
</template>

<style lang="scss">
.game {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}
</style>

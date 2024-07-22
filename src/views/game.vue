<script setup>
import Board from "@/components/game/Board.vue";
</script>
<template>
  <div class="game">
    <div class="layout-game">
      <div class="b1-game">
        <Board></Board>
      </div>
      <div class="b2-game"></div>
    </div>
  </div>
</template>

<style lang="scss">
.game {
  height: 100vh;
  padding: 2rem;
}

.layout-game {
  display: flex;
  height: 100%;
}

.b1-game,
.b2-game {
  flex: 1;
  gap: 1rem;
  height: 100%;
}

.b1-game {
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>

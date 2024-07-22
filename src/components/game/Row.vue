<script setup>
const props = defineProps({
  position: String,
});
</script>
<template>
  <div :class="`row ${position}`">
    <slot></slot>
  </div>
</template>

<style lang="scss">
$size: 120px;

.row {
  height: $size;
  width: 100%;
  background-color: rgba(0, 128, 0, 0.385);
  position: absolute;
  left: 0;
  right: 0;
  display: flex;

  &.left {
    right: auto;
    left: 0;
    height: 100%;
    width: $size;
  }

  &.right {
    left: auto;
    right: 0;
    height: 100%;
    width: $size;
  }

  &.bottom {
    top: auto;
    bottom: 0;
    flex-direction: column;
  }

  &.top {
    top: 0;
    bottom: auto;
  }
}
</style>

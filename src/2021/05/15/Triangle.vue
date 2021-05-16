<template>
  <div class="triangle">
    <div v-for="i in 6" class="triangle__line">
      <span v-for="j in i" class="triangle__cell"></span>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.triangle {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  box-sizing: border-box;
  margin: 0;
  width: 100%;
  height: 100%;

  &__line {
    display: flex;
    justify-content: center;
    width: 100%;
  }

  &__cell {
    $D: 10%;
    $gap: 2px;

    // Draw a perfect circle
    width: $D;
    padding-top: $D;
    border-radius: 9999px;

    box-sizing: border-box;
    margin: $gap;
    margin-left: 2 * $gap;
    margin-right: 2 * $gap;

    background: lightgreen;

    &:first-child,
    &:last-child {
      background-color: lightcoral;
    }
  }
}
</style>
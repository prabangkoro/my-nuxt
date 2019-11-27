<template>
  <div class="box">
    <div class="d-flex align-center justify-center display-1 text-center font-weight-light" style="height: 100%;">
      <slot></slot>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.box {
  background-color: rgba($color: #fff, $alpha: .75);
  height: 80%;
  width: 80%;
}
</style>

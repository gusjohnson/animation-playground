<template>
  <div>
    <h2>Animation 1 Placeholder</h2>
    <div :style="inlineStyle" class="cat" />
  </div>
</template>

<script>
export default {
  name: 'Animation1',
  data() {
    return {
      catPath: require('@/assets/sprites-cat-running.png')
    }
  },
  computed: {
    inlineStyle() {
      return `background-image: url(${this.catPath});`
    }
  }
}
</script>

<style lang="scss">
.cat {
  position: absolute;
  z-index: 1000;
  width: 512px;
  height: 256px;
  background-size: auto;
  // animation-duration: .8s;
  // animation-timing-function: steps(10);
  // animation-iteration-count: infinite;
  // transform: scale(.7);
  // top: 138px;
  // will-change: auto;
}
// @keyframes idle {
//   from { background-position: 0 0; }
//   to { background-position: -5345px 0; }
// }
// @keyframes heal {
//   from { background-position: 0 -534px; }
//   to { background-position: -5345px -534px; }
// }
// @keyframes attacking {
//   from { background-position: 0 2139px; }
//   to { background-position: -5345px 2139px; }
// }
// @keyframes specialAttacking {
//   from { background-position: 0 1602px; }
//   to { background-position: -5345px 1602px; }
// }
// @keyframes dying {
//   from { background-position: 0 -2138px; }
//   to { background-position: -5345px -2138px; }
// }
</style>
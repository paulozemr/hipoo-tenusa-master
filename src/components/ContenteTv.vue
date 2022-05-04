<script>
export default {
  methods: {
    desenha(p0, p1, p2) {
      var canvasElement = document.querySelector("#myCanvas");
      var context = canvasElement.getContext("2d");

      // the triangle
      context.beginPath();
      context.moveTo(p0, p0);
      context.lineTo(p0, p1);
      context.lineTo(p2, p1);
      context.closePath();

      // the outline
      context.lineWidth = 20;
      context.strokeStyle = "#666666";
      context.stroke();

      // the fill color
      context.fillStyle = "#50F";
      context.fill();
    },
  },
  mounted() {
    this.desenha(50, 200, 400);
  },
};
</script>
<template>
  <main id="content">
    <canvas id="myCanvas" width="500" height="500"></canvas>
  </main>
</template>
<style>
main {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>

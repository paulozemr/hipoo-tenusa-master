<script>
import { onMounted } from "vue";

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
      context.lineWidth = 40;
      context.strokeStyle = '#666666';
      context.stroke();

      // the fill color
      context.fillStyle = "#50F";
      context.fill();
    }
  },
  mounted() {
    this.desenha(50, 200, 400)
  }
}
</script>
<template>
  <main id="content">
    <!-- <div id="triangulo-para-cima">
      <p id="hipotenusa"></p>
      <p id="oposto">5</p>
      <p id="adjacente">6</p>
    </div> -->
    <canvas id="myCanvas" width="500" height="500"></canvas>
  </main>
</template>
<style>
div {
  display: inline-block;
  margin-right: 50px;
}

#triangulo-para-cima {
  width: 0;
  height: 0;
  border-left: 0px solid transparent;
  border-right: 350px solid transparent;
  border-bottom: 280px solid #5386E4;
  margin-left: 600px;
  margin-top: 200px;
}

div #adjacente {
  float: right;
  margin-top: 105px
}

div #oposto {
  float: bottom;
  margin-left: 105px;
}
</style>

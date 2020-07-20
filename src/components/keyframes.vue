<template>
  <div class="stage">
    <div class="box bounce-1"></div>
    <div>
      <button @click="goTest">Test</button>
      <button @click="goHelloWorld">HelloWorld</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
      return{}
  },
  mounted() {},
  methods: {
    goTest() {
      this.$router.push({path: "/Test"});
    },
    goHelloWorld() {
      this.$router.push({path: "/HelloWorld"});
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.stage {
  border-bottom: 3px solid #444;
  display: flex;
  height: 500px;
  width: 100%;
}
.box {
  align-self: flex-end;
  animation-duration: 2s;
  animation-iteration-count: infinite;
  background-color: #f44336;
  height: 200px;
  margin: 0 auto 0 auto;
  transform-origin: bottom;
  width: 200px;
}
.bounce-1 {
  animation-name: bounce-1;
  animation-timing-function: ease;
}
@keyframes bounce-1 {
  0% {
    transform: scale(1, 1) translateY(0);
  }
  10% {
    transform: scale(1.1, 0.9) translateY(0);
  }
  30% {
    transform: scale(0.9, 1.1) translateY(-300px);
  }
  50% {
    transform: scale(1.05, 0.95) translateY(0);
  }
  57% {
    transform: scale(1, 1) translateY(-10px);
  }
  64% {
    transform: scale(1, 1) translateY(0);
  }
  100% {
    transform: scale(1, 1) translateY(0);
  }
}
</style>
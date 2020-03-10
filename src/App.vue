<template>
  <div id="app">
    <h1>Simple Calculator</h1>
    <Calculator />
  </div>
</template>

<script>
import Calculator from './main/Calculator'
export default {
  name: 'App',
  components: { Calculator }
}
</script>

<style lang="scss">
  @font-face {
    font-family: 'RobotoMono';
    src: url('./assets/fonts/RobotoMono-Thin.ttf');
  }
  * {
    font-family: 'RobotoMono', monospace;
  }
  body {
    margin: 0;
  }
  #app {
    display: flex;
    flex-direction: column;
    height: 100vh;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: white;
    background: #012933;
  }
</style>

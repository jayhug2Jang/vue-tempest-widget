<template>
  <main id="main-tag">
  </main>
</template>

<script>


import TempestWidget from "@tempestcgi/tempest-widget";

export default {
  name: 'App',
  components: {

  },
  mounted() {
    const dataForInject = {
      canvasId: 'application-canvas',
      assetPrefix: 'https://showcase.tempest-vr.com/casper/',
      debug: false,
      tools: { sceneMode: true, cameraPosition: true },
      canvasParentId: 'main-tag',
    };

    TempestWidget.widget(dataForInject);

  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

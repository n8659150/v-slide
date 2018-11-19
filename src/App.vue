<template>
  <div id="app">

    <full-page ref="fullpage" id="fullpage" :options="options">
      <div class="section">
        <img src="./assets/logo.png">
        <HelloWorld/>
      </div>
      <div class="section">
        <h3>第二页</h3>
      </div>
      <div class="section">
        <div class="slide">
          <h3>第三页第一张</h3>
        </div>
        <div class="slide">
          <h3>第三页第二张</h3>
        </div>
        <div class="slide">
          <h3>第三页第三张</h3>
        </div>
      </div>
      <div class="section">
        <h3>第四页</h3>
      </div>
      <div class="section">
        <h3>第五页</h3>
      </div>
    </full-page>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";

export default {
    name: "App",
    components: {
        HelloWorld
    },
    data() {
        return {
            options: {
                licenseKey: "OPEN-SOURCE-GPLV3-LICENSE",
                scrollBar: false,
                navigation: true,
                controlArrows: false,
                sectionsColor: []
            }
        };
    }
};
</script>

<style>
#app {
    font-family: "Avenir", Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
}
</style>

<template>
  <div id="app">

    <full-page ref="fullpage" id="fullpage" :options="options">
      <div class="section">
        <!-- cover -->
        <div>
          <div class="title1">Vue.js初探 - 在线翻译App</div>
          <div class="title2">&nbsp;</div>
          <div class="title2">Jack Li</div>
        </div>
      </div>
      <div class="section">
        <HelloWorld />
      </div>
      <div class="section">
        <div>
            <div class="title1">大纲</div>
            <div class="title2">&nbsp;</div>
            <div class="title2" style="text-align:left;margin-left:10%;">-<span style="display:inline-block; width:25px;height:10px;"></span> Vue.js 简介</div>
            <div class="title2">&nbsp;</div>
            <div class="title2" style="text-align:left;margin-left:10%;">-<span style="display:inline-block; width:25px;height:10px;"></span> Vue.js 生态圈</div>
            <div class="title2">&nbsp;</div>
            <div class="title2" style="text-align:left;margin-left:10%;">-<span style="display:inline-block; width:25px;height:10px;"></span> Vue.js CLI + 项目结构简介</div>
            <div class="title2">&nbsp;</div>
            <div class="title2" style="text-align:left;margin-left:10%;">-<span style="display:inline-block; width:25px;height:10px;"></span> 在线翻译App 源代码分析</div>
          </div>
      </div>
      <div class="section">
        <!-- content page -->
        <div class="slide">
          <div>
            <div class="title1">Vue.js 简介</div>
          </div>
        </div>
        <div>
          <div>
            <div class="title1">大纲</div>
            <div class="title2">&nbsp;</div>
            <div class="title2">Vue.js 简介</div>
            <div class="title2">&nbsp;</div>
            <div class="title2">Vue.js - 生态圈</div>
            <div class="title2">&nbsp;</div>
            <div class="title2">Vue.js - CLI + 项目结构简介</div>
            <div class="title2">&nbsp;</div>
            <div class="title2">源代码分析 - 在线翻译App</div>
          </div>
        </div>
        <div class="slide">
          <div class="title1">Vue.js</div>
          <div class="title2">Vue 官方推荐的项目脚手架工具</div>
          <div class="title3">小标题及文字内容
            <br>副文字内容</div>
          <div class="DownloadBtn">
            <a href="#" target="_blank">查看代码</a>
          </div>
        </div>
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
/* #app {
    font-family: "Avenir", Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
} */
</style>

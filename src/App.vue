<template>
  <div id="app">

    <full-page ref="fullpage" id="fullpage" :options="options">
      <div class="section">
        <!-- cover -->
        <Cover toppingTitle="VUE.JS INTRO" :slideTitle="slideConfig.slideTitle" :authorName="slideConfig.authorName"></Cover>
      </div>
      <div class="section">
        <div class="slide">
          <SingleTitlePage toppingTitle="OVERVIEW" content="大 纲"></SingleTitlePage>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage toppingTitle="INTRO" content="Vue.js 简介"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage toppingTitle="ECOSYSTEM" content="Vue.js 生态圈"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage toppingTitle="PROJECT STRUCTURE" content="项目结构简介"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage toppingTitle="DEMO SOURCECODE" content="Demo源代码分析"></SingleTitlePage>
          </div>
        </div>
      </div>
      <div class="section">
       <DotPointPage pageTitle="大 纲" dotPointStyle="-" :contentArray="slideConfig.dotPointContents"></DotPointPage>
      </div>
      <div class="section">
        <MainContentPage mainTitle="Vue CLI" subTitle="Vue 官方推荐的项目脚手架工具" description1="小标题及文字内容" description2="副文字内容" buttonText="查看源码" buttonLink="http://www.jackyangli.com"></MainContentPage>
      </div>
    </full-page>
  </div>
</template>

<script>
import Cover from "@/components/Cover";
import SingleTitlePage from "@/components/SingleTitlePage"
import DotPointPage from "@/components/DotPointPage"
import MainContentPage from "@/components/MainContentPage"
export default {
    name: "App",
    components: {
        Cover,
        SingleTitlePage,
        DotPointPage,
        MainContentPage
    },
    data() {
        return {
            options: {
                licenseKey: "OPEN-SOURCE-GPLV3-LICENSE",
                scrollBar: false,
                navigation: true,
                controlArrows: false,
                sectionsColor: []
            },
            slideConfig:{
              slideTitle:"Vue.js初探",
              authorName:"Jack Li",
              dotPointContents:["Vue.js 简介","Vue.js 生态圈","项目结构简介","Demo源代码分析"]
            },

        };
    },
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

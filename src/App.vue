<template>
  <div id="app">
    <full-page ref="fullpage" id="fullpage" :options="options">
      <div class="section">
        <!-- cover -->
        <Cover
          toppingTitle="VUE.JS INTRO"
          :slideTitle="slideConfig.slideTitle"
          :authorName="slideConfig.authorName"
        ></Cover>
      </div>
      <div class="section">
        <div class="slide">
          <SingleTitlePage toppingTitle="OVERVIEW" :contentArray="[{text:'大 纲', fontSize:'180'}]"></SingleTitlePage>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="INTRO"
              :contentArray="[{text:'Vue.js 简介', fontSize:'180'}]"
            ></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="ECOSYSTEM"
              :contentArray="[{text:'Vue.js 生态圈', fontSize:'180'}]"
            ></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="PROJECT STRUCTURE"
              :contentArray="[{text:'项目结构简介', fontSize:'180'}]"
            ></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="DEMO SOURCECODE"
              :contentArray="[{text:'Demo源代码分析', fontSize:'180'}]"
            ></SingleTitlePage>
          </div>
        </div>
      </div>

      <div class="section">
        <DotPointPage
          pageTitle="大 纲"
          dotPointStyle="-"
          :contentArray="slideConfig.dotPointContents"
        ></DotPointPage>
      </div>

      <div class="section">
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="INTRO"
              :contentArray="[{text:'Vue.js 简介', fontSize:'180'}]"
            ></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="SINCE 2014"
              :contentArray="[{text:'2014年,尤雨溪', fontSize:'180'}]"
            ></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="HIGHLIGHTS"
              :contentArray="[{text:'MVVM,V-DOM,模块化', fontSize:'160'}]"
            ></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="WHY VUE.JS"
              :contentArray="[{text:'AngularJS指令 + React模块化 = Vue.js', fontSize:'100'}]"
            ></SingleTitlePage>
          </div>
        </div>
      </div>

      <div class="section">
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="ECOSYSTEM"
              :contentArray="[{text:'Vue.js 生态圈',fontSize:'180'}]"
            ></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="SCAFFOLDING"
              :contentArray="[{text:'Vue CLI',fontSize:'180'}, {text:'- 项目脚手架工具',fontSize:'72'}]"
            ></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="ROUTER"
              :contentArray="[{text:'Vue-Router', fontSize:'180'}, {text:'- 路由库', fontSize:'72'}]"
            ></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="HTTP REQUEST PACK"
              :contentArray="[{text:'Vue-resource', fontSize:'180'}, {text:'- Vue.js 1.x http库', fontSize:'72'}]"
            ></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="HTTP REQUEST PACK"
              :contentArray="[{text:'Axios', fontSize:'180'}, {text:'- Vue.js 2.x http库', fontSize:'72'}]"
            ></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="3RD PARTY COMPONENT LIBS"
              :contentArray="[{text:'element-ui、at-ui...',fontSize:'180'}, {text:'- UI组件库', fontSize:'72'}]"
            ></SingleTitlePage>
          </div>
        </div>
      </div>

      <div class="section">
        <MainContentPage
          mainTitle="Vue CLI"
          subTitle="Vue 官方推荐的项目脚手架工具"
          description1="小标题及文字内容"
          description2="副文字内容"
          buttonText="查看源码"
          buttonLink="http://www.jackyangli.com"
        ></MainContentPage>
      </div>
    </full-page>
  </div>
</template>

<script>
import Cover from "@/components/Cover";
import SingleTitlePage from "@/components/SingleTitlePage";
import DotPointPage from "@/components/DotPointPage";
import MainContentPage from "@/components/MainContentPage";
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
      slideConfig: {
        slideTitle: "Vue.js初探",
        authorName: "Jack Li",
        dotPointContents: [
          "Vue.js 简介",
          "Vue.js 生态圈",
          "项目结构简介",
          "Demo源代码分析"
        ]
      }
    };
  }
};
</script>

<style>
</style>

<template>
  <div id="app">

    <full-page ref="fullpage" id="fullpage" :options="options">
      <div class="section">
        <!-- cover -->
        <Cover topping-title="VUE.JS INTRO" :slide-title="slideConfig.slideTitle" :author-name="slideConfig.authorName"></Cover>
      </div>
      <div class="section">
        <div class="slide">
          <SingleTitlePage topping-title="OVERVIEW" :content-array="[{text:'大 纲', fontSize:'180'}]"></SingleTitlePage>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="INTRO" :content-array="[{text:'Vue.js 简介', fontSize:'180'}]"></SingleTitlePage>
          </div>
        </div>
        
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="ECOSYSTEM" :content-array="[{text:'Vue.js 生态圈', fontSize:'180'}]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="PROJECT STRUCTURE" :content-array="[{text:'项目结构简介', fontSize:'180'}]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="DEMO SOURCECODE" :content-array="[{text:'Demo源代码分析', fontSize:'180'}]"></SingleTitlePage>
          </div>
        </div>
      </div>

      <!-- <div class="section">
       <DotPointPage page-title="大 纲" dot-point-style="-" :content-array="slideConfig.dotPointContents"></DotPointPage>
      </div> -->

      <div class="section">
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="INTRO" :content-array="[{text:'Vue.js 简介',fontSize:'180'}]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="SINCE 2014" :content-array="[{text:'2014年',fontSize:'180'},{text:'尤雨溪',fontSize:'180'}]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="HIGHLIGHTS" :content-array="[{text:'MVVM',fontSize:'180'},{text:'Virtual DOM',fontSize:'180'},{text:'模块化',fontSize:'180'}]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="WHY VUE.JS" :content-array="[{text:'ngJS - 指令',fontSize:'180'}, {text:'+ React - 模块化',fontSize:'180'}, {text:'= Vue.js',fontSize:'180'}]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="MEMEs" :content-array="[{text:'Angulareact.js',fontSize:'180'}]"></SingleTitlePage>
          </div>
        </div>
      </div>

      <div class="section">
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="ECOSYSTEM" :content-array="[{text:'Vue.js 生态圈',fontSize:'180'}]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="SCAFFOLDING" :content-array="[{text:'Vue CLI',fontSize:'180'}, {text:'- 项目脚手架工具',fontSize:'80'}]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="ROUTER" :content-array="[{text:'Vue-Router',fontSize:'180'}, {text:'- 路由库',fontSize:'80'}]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="HTTP REQUEST PACK" :content-array="[{text:'Vue-resource',fontSize:'180'}, {text:'- Vue.js 1.x http库',fontSize:'80'}]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="HTTP REQUEST PACK" :content-array="[{text:'Axios',fontSize:'180'}, {text:'- Vue.js 2.x http库',fontSize:'80'}]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="3RD PARTY COMPONENT LIBS" :content-array="[{text:'element-ui、at-ui...',fontSize:'180'}, {text:'- UI组件库',fontSize:'80'}]"></SingleTitlePage>
          </div>
        </div>
      </div> 
      
      <div class="section">
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="PROJECT STRUCTURE" :content-array="[{text:'项目结构简介', fontSize:'180'}]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="PROJECT ELEMENTS - OVERVIEW" :content-array="[{text:'+ src folder',fontSize:'120'}, {text:'+ static folder',fontSize:'120'},{text:'index.html',fontSize:'120'},{text:'package.json',fontSize:'120'}]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="PROJECT ELEMENTS - SRC" :content-array="[{text:'- src',fontSize:'120'}, {text:'+ assets folder',fontSize:'80'}, {text:'+ components folder',fontSize:'80'}, {text:'App.vue',fontSize:'80'}, {text:'main.js',fontSize:'80'} ]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="PROJECT ELEMENTS - ASSETS" :content-array="[{text:'- assets',fontSize:'120'}, {text:'logo.png',fontSize:'80'} ]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="PROJECT ELEMENTS - COMPONENTS" :content-array="[{text:'- components',fontSize:'120'}, {text:'HelloWorld.vue',fontSize:'80'} ]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="PROJECT ELEMENTS - APP.VUE" :content-array="[{text:'App.vue',fontSize:'120'}, {text:'<template> ... </template>',fontSize:'100'},{text:'<script> ... </script>',fontSize:'100'}, {text:'<style> ... </style>',fontSize:'100'}]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="PROJECT ELEMENTS - APP.VUE" :content-array="[{text:'template tag - HTML',fontSize:'120'}, {text:'<template>',fontSize:'100'},{text:'<HelloWorld></HelloWorld>',fontSize:'100'}, {text:'</template>',fontSize:'100'}]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="PROJECT ELEMENTS - APP.VUE" :content-array="[{text:'script tag - JS',fontSize:'120'}, {text:'<script>',fontSize:'100'},{text:'import HelloWorld from ../HelloWorld.vue' ,fontSize:'80'}, {text:'</script>',fontSize:'100'}]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="PROJECT ELEMENTS - APP.VUE" :content-array="[{text:'style tag - CSS',fontSize:'120'}, {text:'<style>',fontSize:'100'},{text:'h3 { font-size: 1.6 rem}' ,fontSize:'80'}, {text:'</style>',fontSize:'100'}]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="PROJECT ELEMENTS - INDEX.HTML" :content-array="[{text:'index.html - 架子',fontSize:'120'}, {text:'<body>',fontSize:'100'},{text:'<App></App>' ,fontSize:'80'}, {text:'</body>',fontSize:'100'}]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage topping-title="PROJECT ELEMENTS - MAIN.JS" :content-array="[{text:'main.js - 入口文件',fontSize:'120'}, {text:'new Vue({...})',fontSize:'100'}]"></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <MainContentPage main-title="Vue CLI" sub-title="Vue 官方推荐的项目脚手架工具" description1="开箱即用" description2="Let's GO" button-text="查看项目结构" button-link="https://github.com/n8659150/v-slide"></MainContentPage>
          </div>      
        </div>
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

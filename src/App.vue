<template>
  <div id="app">
    <full-page ref="fullpage" id="fullpage" :options="options">
      <div class="section">
        <!-- cover -->
        <Cover
          toppingTitle="Translation App In 30 Mins"
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
              toppingTitle="WHAT HAPPENED"
              :contentArray="[{text:'动机,漫谈', fontSize:'180'}]"
            ></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="HOW TO MAKE IT HAPPEN"
              :contentArray="[{text:'功能,原理', fontSize:'180'}]"
            ></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="MAKE IT HAPPEN"
              :contentArray="[{text:'放码过来', fontSize:'180'}]"
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
              toppingTitle="LEARN IN 21 DAYS"
              :contentArray="[{text:'21天精通XXX', fontSize:'180'}]"
            ></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="LESS TIME"
              :contentArray="[{text:'周期越来越短', fontSize:'150'}, {text:'- 21天，10天，3天',fontSize:'60'}]"
            ></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="LEARN REGEX 30 MIN"
              :contentArray="[{text:'30分钟精通正则？', fontSize:'150'}]"
            ></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="I WANT MONEY"
              :contentArray="[{text:'老板：我要变现！', fontSize:'150'},{text:'- 员工：给我钱，帮你变现',fontSize:'60'}]"
            ></SingleTitlePage>
          </div>
        </div>
      </div>

      <div class="section">
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="CRAZY IT FIELD"
              :contentArray="[{text:'打了鸡血的互联网',fontSize:'150'}]"
            ></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="RAMDON PEOPLE COMING IN"
              :contentArray="[{text:'想致富，做码农',fontSize:'150'}, {text:'- 建筑，化工，生物全员转行',fontSize:'60'}]"
            ></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="COST OF PROGRAMMING"
              :contentArray="[{text:'编程成本越来越低', fontSize:'150'}, {text:'- 全员编程时代', fontSize:'60'}]"
            ></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="WHERE IS THE VALUE"
              :contentArray="[{text:'程序员的价值？', fontSize:'150'}, {text:'- 别人5K 你10K，凭什么', fontSize:'60'}]"
            ></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="VALUES"
              :contentArray="[{text:'创意？人脉？听话？', fontSize:'150'}]"
            ></SingleTitlePage>
          </div>
        </div>
        <div class="slide">
          <div>
            <SingleTitlePage
              toppingTitle="MAKE IT HAPPEN"
              :contentArray="[{text:'Make Your Idea Happen',fontSize:'150'}]"
            ></SingleTitlePage>
          </div>
        </div>
      </div>

      
      <!-- <div class="section">
        <MainContentPage
          mainTitle="Vue CLI"
          subTitle="Vue 官方推荐的项目脚手架工具"
          description1="小标题及文字内容"
          description2="副文字内容"
          buttonText="查看源码"
          buttonLink="http://www.jackyangli.com"
        ></MainContentPage>
      </div> -->
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
        slideTitle: "30分钟实现翻译APP",
        authorName: "Jack Li",
        dotPointContents: [
          "漫谈：21天的梗, 3天的梗，30分钟的梗",
          "漫谈：打了鸡血的互联网",
          "漫谈：MVP, Fail Fast",
          "放码过来：构思，实现"
        ]
      }
    };
  }
};
</script>

<style>
</style>

<template>
  <div>
    <div class="title3 toppingTitle">{{toppingTitle}}</div>
     <div v-for="(content,index,$key) in contentArray" :key="$key">
        <div class="single-title-page">{{content}}</div>
     </div>
    <div class="title2">&nbsp;</div>
  </div>
</template>

<script>
export default {
    name: "SingleTitlePage",
    data() {
        return {
            msg: ""
        };
    },
    props: ["contentArray","subTitle","toppingTitle"]
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.single-title-page {
    font-size: 180px;
}

</style>

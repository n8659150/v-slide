<template>
  <div>
    <div class="title3 toppingTitle">{{toppingTitle}}</div>
     <div v-for="(content,index,$key) in contentArray" :key="$key">
        <div :style="{fontSize: content.fontSize + 'px'}">{{content.text}}</div>
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
</style>

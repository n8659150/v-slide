<template>
  <div>
    <div class="title3 toppingTitle">{{toppingTitle}}</div>
    <div class="slide-title">{{slideTitle}}</div>
    <div class="title2">&nbsp;</div>
    <div class="title2">&nbsp;</div>
    <div class="title2 author-title">{{authorName}}</div>
  </div>
</template>

<script>
export default {
    name: "Cover",
    data() {
        return {
            msg: ""
        };
    },
    props: ["toppingTitle","slideTitle", "authorName"]
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.slide-title {
    font-size: 140px;
}

.author-title {
    font-size: 44px;
}
</style>

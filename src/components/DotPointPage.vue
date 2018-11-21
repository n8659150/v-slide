<template>
    <div>
        <div class="title1">{{pageTitle}}</div>
        <div v-for="(content,index,$key) in contentArray" :key="$key">
            <div class="title2">&nbsp;</div>
            <div class="title2" style="text-align:left;margin-left:10%;">
                {{dotPointStyle}} <span class="divider"></span> {{content}}
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "DotPointPage",
    data() {
        return {
            msg: ""
        }
    },
    props: [
        "pageTitle",
        "contentArray",
        "dotPointStyle"
    ]
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.divider {
    display: inline-block;
    width: 25px;
    height: 10px;
}
</style>

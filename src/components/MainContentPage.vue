<template>
    <!-- content page -->
    <div class="slide">
        <div class="title1">{{mainTitle}}</div>
        <div class="title2">{{subTitle}}</div>
        <div class="title3">
            {{description1}}
            <br/>
            {{description2}}
        </div>
        <div class="DownloadBtn">
            <a :href="buttonLink" target="_blank">{{buttonText}}</a>
        </div>
    </div>
</template>

<script>
export default {
    name: "MainContentPage",
    data() {
        return {
            msg: ""
        };
    },
    props: ["mainTitle", "subTitle", "description1", "description2","buttonText","buttonLink"]
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.slide-title {
    font-size: 72px;
}

.author-title {
    font-size: 44px;
}
</style>

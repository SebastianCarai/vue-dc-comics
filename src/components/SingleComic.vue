<template>

    <!-- Single comic -->
    <div class="comic_container">
        <div class="img_container">
            <img :src="info.thumb" alt="">
        </div>
        <div>{{info.series.toUpperCase()}}</div>
    </div>
    <!-- End single comic -->
</template>

<script>
export default {
    name:'SingleComic',
    props:[
        'info',
    ]
}
</script>

<style scoped lang="scss">
.comic_container{
    width: calc((100% / 6) - 20px);
    height: 200px;
    margin: 10px 10px 30px;
    position: relative;
    .img_container{
        height: inherit;
        width: 100%;
        overflow: hidden;
    }
    div{
        margin-top: 10px;
        font-size: 13px;
    }
}

</style>
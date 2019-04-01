<template>
    <div class="mask-container">
        <div class="title">时尚培训</div>
        <div class="title-f">点击查看</div>
    </div>
</template>

<script>
    export default {
        props: {

        }
    }
</script>

<style scoped lang="less">
    .mask-container {
        position: absolute;
        width: 100%;
        height: 100%;
        left: 0;
        top: 0;
        padding-left: 130%;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        transition: all 0.6s;
        background-color: rgba(0, 0, 0, 0); 
        &:hover {
            padding-left: 0;
             background-color: rgba(0, 0, 0, 0.6); 
        }
        .title {
            font-size: 24px;
            line-height: 30px;
            color: #fff;
        }
        .title-f {
            font-size: 16px;
            line-height: 20px;
            color: #fff;
        }
    }
</style>
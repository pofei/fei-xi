<template>
    <div :class="$style.footer">
        <a :class="$style.txt_span" href="/">
            关于我们
        </a>
        <span :class="$style.line">|</span>
        <a :class="$style.txt_span" href="/">
            加入我们
        </a>
        <span :class="$style.line">|</span>
        <a :class="$style.txt_span" href="/">
            合作伙伴
        </a>
        <span :class="$style.line">|</span>
        <a :class="$style.txt_span" href="/">
            梦想合伙人
        </a>
        <span :class="$style.line">|</span>
        <a :class="$style.txt_span" href="/">
            网站地图
        </a>
        <span :class="$style.line">|</span>
        <a :class="$style.txt_span" href="/">
            服务条款
        </a>
        <span :class="$style.line">|</span>
        <a :class="$style.txt_span" href="/">
            隐私说明
        </a>
        <span :class="$style.line">|</span>
        <a :class="$style.txt_span" href="/">
            版权说明
        </a>
        <span :class="$style.copyright">
            粤ICP备1648948439号 &copy;2018-2020123.com
        </span>

    </div>
</template>

<script>
    export default {
    }
</script>

<style module lang="less">
    .footer {
        height: 132px;
        line-height: 132px;
        text-align: center;
        background-color: #000;
        .txt_span {
            color: #fff;
            font-size: 16px;
            &:hover {
                color: red;
            }
        }
        .line {
            color: #fff;
            font-size: 16px;
            padding: 0 8px;
        }
        .copyright {
            margin-left: 10px;
            color: #fff;
            font-size: 16px;
        }
    }
</style>
<template>
    <div class="slider-tab-container" ref="slider_tab">
        <div :class="containerName">
            <a-anchor class="anchor_link_container" :affix="false" @click="handleClick">
                <a href="/" class="logo_container">
                    <img class="logo" src="../../assets/index/logo.png"/>
                </a>
                <a-anchor-link class="anchor_link" href="#anchor1" title="时尚培训" />
                <a-anchor-link class="anchor_link"  href="#anchor2" title="设计师孵化" />
                <a-anchor-link class="anchor_link"  href="#anchor3" title="时尚活动与发布" />
                <a-anchor-link class="anchor_link"  href="#anchor4" title="产品原创合作" />
                <a-anchor-link class="anchor_link"  href="#anchor5" title="供应链" />
                <a-anchor-link class="anchor_link"  href="#anchor6" title="智慧工场" />
                <a-anchor-link class="anchor_link"  href="#anchor7" title="销售平台" />
            </a-anchor>
        </div>
    </div>
</template>

<script>
    export default {
        data(){
            return{
                affix: false
            }
        },
        computed: {
            containerName() {
                return this.affix ? 'anchor-container-wrapper' : 'anchor-container-wrapper fixedContainer'
            }
        },
        mounted() {
            window.addEventListener('scroll', this.checkAffix, false);
           
        },
        beforeDestroy() {
            window.removeEventListener('scroll', this.checkAffix.bind(this), false);
        },
        methods:{
            handleClick (e) {
                e.preventDefault();
            },
            checkAffix () {
                const top = document.querySelector('.slider-tab-container').offsetTop;
                const scrollTop = document.documentElement.scrollTop || document.body.scrollTop || 0;
                if(top >= scrollTop) {
                    this.affix = true;
                }else {
                    this.affix = false;
                }
            }
        }
    }
</script>

<style scoped lang="less">
    .slider-tab-container {
        height: 107px;
        line-height: 107px;
        background-color: #fff;
        .anchor-container-wrapper {
            border-bottom: 3px solid #e9e9e9;
            height: 107px; 
            width: 100%;
            &.fixedContainer {
                position: fixed;
                z-index: 10;
                left: 0;
                top: 0;
                width: 100%;
                background: #fff;
                .logo_container {
                    margin-left: 0;
                }
            }
        }
        .anchor_link_container {
            width: 1318px;
            margin: 0 auto;
            height: 104px; 
            .logo_container {
                width: 170px;
                margin-top: 25px;
                padding-right: 30px;
                display: block;
                float: left;
                margin-left: -180px;
                transition: all .3s;
                .logo {
                    width: 100%;
                }
            }
            
            .ant-anchor-ink {
                display: none;
            }  
            /deep/.anchor_link {
                float: left;
                margin-right: 30px;
                height: 104px;
                line-height: 104px;
                color: #40434a;
                font-size: 24px;
                padding: 0;
                /deep/.ant-anchor-link-title-active {
                    color: #e60012;
                }
                
                /deep/.ant-anchor-link-title {
                    text-decoration: none!important;
                    &:hover {
                        color: #e60012;
                    }
                }
            }
        }
    }
</style>

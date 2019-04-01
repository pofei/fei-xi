<template>
    <div :class="$style.header">
        <a :class="$style.logo" href="/">
            <img src="../assets/index/logo.png" alt="">
        </a>
        <div :class="$style.search_icon">
            <img src="../assets/index/search-icon.png" :class="$style.search_icon_img" alt="">
        </div>
        <div :class="$style.tabList">
            <div :class="$style.item">
                <DropMenu title="产业解决方案" :menuList="menuList1"/>
            </div>
            <div :class="$style.item">
                <DropMenu title="红T智库" :menuList="menuList2"/>
            </div>
            <div :class="$style.item">
                <DropMenu title="时尚圈" :menuList="menuList2"/>
            </div>
            <div :class="$style.item">
                <DropMenu title="供应链云平台" :menuList="menuList1"/>
            </div>
        </div>

    </div>
</template>

<script>
import DropMenu from './Home/dropMenu.vue'
export default {
  data () {
    return {
      menuList1: [
        {
          text: '设计名师',
          link: '/'
        },
        {
          text: '原创产品认证',
          link: 'https://whjh.maker-ip.com/app/whjhIndex'
        }, {
          text: '共享版房',
          link: '/'
        }, {
          text: '智慧工厂',
          link: '/'
        }, {
          text: '时尚定制',
          link: '/'
        }, {
          text: '线上销售',
          link: '/'
        }, {
          text: '线下品牌推广',
          link: '/'
        }, {
          text: '服装大数据',
          link: '/'
        }, {
          text: '红T时尚创意园区',
          link: '/'
        }
      ],
      menuList2: [
        {
          text: '时尚培训',
          link: '/'
        },
        {
          text: '国内时尚界',
          link: '/'
        }, {
          text: '国际合作',
          link: '/'
        }, {
          text: '全球知名教师',
          link: '/'
        }, {
          text: '设计资源共享',
          link: '/'
        }, {
          text: '设计软件协作',
          link: '/'
        }
      ]
    }
  },
  components: {
    DropMenu
  }

}
</script>

<style module lang="less">
    .header {
        height: 100px;
        background: #fff;
        .logo {
            width: 140px;
            float: left;
            margin-top: 31px;
            margin-left: 20px;
            img {
                display: block;
                width: 100%;
                height: 100%;
            }
        }
        .tabList {
            float: right;
            line-height: 100px;
            height: 100px;
            .item {
                float: left;
                height: 100px;
                line-height: 100px;
                cursor: pointer;
                color: #000;
                font-size: 24px;
                padding: 0 10px;
                &:hover {
                    color: red;
                }
            }
        }
        .search_icon {
            float: right;
            width: 50px;
            height: 100px;
            position: relative;
            cursor: pointer;
            .search_icon_img {
                width: 22px;
                height: 22px;
                position: absolute;
                left: 50%;
                top: 50%;
                transform: translate(-50%, -50%);
            }
        }
    }
</style>

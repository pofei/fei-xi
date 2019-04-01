<template>
  <a-dropdown>
    <a class="ant-dropdown-link" href="javascript:void(0);">
      {{title}}
    </a>
    <a-menu slot="overlay">
       <a-menu-item v-for="(item,index) in menuList" :key="index">
            <a :href="item.link">{{item.text}}</a>
        </a-menu-item>
    </a-menu>
  </a-dropdown>
</template>

<script>
export default {
  props: [
    'title',
    'menuList'
  ]
}
</script>

<style scoped lang="less">
    .ant-dropdown-link {
        color: #000;
        text-decoration: none!important;
        padding: 5px 20px;
        transition: none;
        transition: background-color 0.2s;
        &:hover {
            color: white;
            background: red;
        }

    }
    .ant-dropdown-menu-item:hover,
    .ant-dropdown-menu-submenu-title:hover {
        background-color: red;
        color: #fff;
        > a {
            color: #fff;
        }
    }
</style>

<template>
  <div class="tab_choose">
    <label for>{{list.title}} :</label>
    <span
      :key="index"
      :class="active === index ? 'active' :0"
      v-for="(item,index) in list.list"
      @click="handleChange(index)"
    >{{item}}</span>
  </div>
</template>

<script>
export default {
  props: {
    list: {
      type: Object
    }
  },
  name: 'tab',
  data () {
    return {
      arr: ['全部', '今天', '明天', '本周', '本周末', '本月'],
      active: 0
    }
  },
  methods: {
    handleChange (index) {
      this.active = index
    }
  }
}
</script>

<style lang="less" scoped>
.tab_choose {
  padding-top: 20px;
  padding-bottom: 20px;
  font-size: 20px;
  color: #727272;
  label {
    margin-right: 13px;
  }
  span {
    margin-right: 10px;
    cursor: pointer;
    padding: 7px 16px;
    border: 1px solid transparent;
    border-radius: 5px;
  }
  span:last-child{
    margin-right: 0;
  }
  span.active {
    color: #cfa972;
    border: 1px solid #cfa972;
  }
}
</style>

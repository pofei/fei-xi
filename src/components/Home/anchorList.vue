<template>
  <div class="cloths-container">
    <h5>服装产业链全汇聚</h5>
    <p>Garment industry chain</p>
    <div class="anchor_link_list">
      <a-anchor wrapperClass="anchor_link_container" :affix="false" @click="handleClick">
        <a-anchor-link class="anchor_link" href="#anchor1">
          <div class="anchor_wrapper" slot="title">
            <img src="../../assets/index/c1.png" alt>
            <span>时尚培训</span>
          </div>
        </a-anchor-link>
        <a-anchor-link class="anchor_link" href="#anchor2">
          <div class="anchor_wrapper" slot="title">
            <img src="../../assets/index/c2.png" alt>
            <span>设计师孵化</span>
          </div>
        </a-anchor-link>
        <a-anchor-link class="anchor_link" href="#anchor3">
          <div class="anchor_wrapper" slot="title">
            <img src="../../assets/index/c3.png" alt>
            <span>时尚活动与发布</span>
          </div>
        </a-anchor-link>
        <a-anchor-link class="anchor_link" href="#anchor4">
          <div class="anchor_wrapper" slot="title">
            <img src="../../assets/index/c4.png" alt>
            <span>产品原创合作</span>
          </div>
        </a-anchor-link>
        <a-anchor-link class="anchor_link" href="#anchor5">
          <div class="anchor_wrapper" slot="title">
            <img src="../../assets/index/c5.png" alt>
            <span>供应链</span>
          </div>
        </a-anchor-link>
        <a-anchor-link class="anchor_link" href="#anchor6">
          <div class="anchor_wrapper" slot="title">
            <img src="../../assets/index/c6.png" alt>
            <span>智慧工场</span>
          </div>
        </a-anchor-link>
        <a-anchor-link class="anchor_link" href="#anchor7">
          <div class="anchor_wrapper" slot="title">
            <img src="../../assets/index/c7.png" alt>
            <span>销售平台培训</span>
          </div>
        </a-anchor-link>
      </a-anchor>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  methods: {
    handleClick(e) {
      e.preventDefault();
    }
  }
};
</script>

<style scoped lang="less">

.cloths-container {
  height: 720px;
  width: 1318px;
  margin: 0 auto;
  h5 {
    font-size: 30px;
    color: #000;
    margin-top: 100px;
    text-align: left;
    margin-bottom: 0;
  }
  p {
    font-size: 18px;
    color: #000;
    line-height: 30px;
    text-align: left;
    margin-bottom: 0;
  }
  .anchor_link_list {
    .anchor_link_container {
        overflow: hidden;
        .anchor_link {
            float: left;
            width: 298px;
            padding: 0;
            height: 140px;
            margin-top: 80px;
            position: relative;
            cursor: pointer;
        }
    }  
    .anchor_wrapper {
      width: 298px;
      height: 140px;
      position: relative;
      cursor: pointer;
      img {
        display: block;
        margin: 0 auto;
      }
      span {
        display: block;
        text-align: center;
        position: absolute;
        bottom: 0;
        left: 50%;
        transform: translateX(-50%);
        font-size: 24px;
        color: #2f2e2e;
      }
    }
  }
}
</style>
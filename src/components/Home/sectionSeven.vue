<template>
  <div>
    <h3 id="anchor7">
      <div class="seven">
        <div class="gy_index">07</div>
        <div class="gy_orange"></div>
        <div class="gy_title">销售平台</div>
        <div class="gy_title_eg">sales platform</div>
        <ul class="content">
          <li>为设计师提供多渠道销售模式</li>
          <li>—在线虚拟时装周活动</li>
          <li>—为设计师提供各类时尚活动资讯以便参考</li>
          <li>—将线下设计师沙龙、峰会与线上论坛、实况直播相融合</li>
          <li>—线上销售店铺:至上集</li>
          <li>—服装销售大数据平台</li>
        </ul>
        <div class="plat_content">
          <div class="pic relative">
            <MaskContainer/>
            <img src="../../assets/index/ssz6.jpg" alt>
          </div>
          <div class="pic relative">
            <MaskContainer/>
            <img src="../../assets/index/ssz7.jpg" alt>
          </div>
          <div class="pic relative">
            <MaskContainer/>
            <img src="../../assets/index/ssz8.jpg" alt>
          </div>
        </div>
      </div>
    </h3>
  </div>
</template>

<script>
import MaskContainer from '../../components/Home/mask.vue';

export default {
    components: {
        MaskContainer
    }
};
</script>

<style scoped lang="less">
.relative {
  position: relative;
  overflow: hidden;
}
 .same_content{
    width:1200px;
    overflow: hidden;
    margin: 0 auto;
    margin-bottom:287px;
    .orange{
      display: block;
      width:8px;
      height:50px;
      background:#cfa972;
    }
    .small_orange{
      display: block;
      width:48px;
      height:3px;
      background:#cfa972;
    }
    .title{
      font-size:30px;
      color:#000;
    }
    .title_english{
      font-size:18px;
      color:#000;
    }
    .content{
      font-size:16px;
      color:#0d0d0d;
      line-height: 30px;
    }
    .look_more{
      font-size:16px;
      font-weight: bold;
      color:#333;
    }
    &.content_right{
      position:relative;
      text-align: right;
      .orange{
        margin-left:590px;
      }
      .small_orange{
        margin-left:552px;
      }
    }
    .son{
      float: left;
      width:600px;

    }
    .pic_box{
      margin-top:57px;
      width:100%;
      overflow: hidden;
      .pic{
        width:288px;
        float:left;
        position: relative;
        &.te{
          margin-right:24px;
        }
        img{
          width:100%;
          height:196px;
        }
      }
    }
    .son_right{

      width:580px;
      margin:0 10px;
      img{
        width:100%;
      }
    }
  }
  .seven{
    .gy_index{
      font-size:30px;
      color:#000;
      text-align: center;
    }
    .gy_orange{
      display: block;
      width:8px;
      height:50px;
      background:#cfa972;
      margin:0 auto;
    }
    .gy_title{
      font-size:30px;
      color:#000;
      text-align: center;
    }
    .gy_title_eg{
      font-size:18px;
      color:#000;
      text-align: center;
    }
    .content{
      font-size:16px;
      color:#0d0d0d;
      line-height: 30px;
      text-align: center;
      margin-top:30px;
    }
    .plat_content{
      margin-top:50px;
      margin-bottom:100px;
      width:1300px;
      margin:0 auto;
      overflow: hidden;
      .pic{
        float:left;
        img{
          width: 100%;
        }
        &:nth-of-type(1){
          width:44%;
        }
        &:nth-of-type(2){
          width:21%;
          margin:0 10px;
        }
        &:nth-of-type(3){
          width:32%;
          margin-top:80px;
        }
      }
    }
  }
</style>
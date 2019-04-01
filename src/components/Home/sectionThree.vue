<template>
  <div>
    <h3 id="anchor3">
      <div class="three same_content content_right">
        <div class="son_right son">
          <div class="pic relative">
            <MaskContainer/>
            <img src="../../assets/index/ssz.jpg" alt>
          </div>
        </div>
        <div class="son_left son">
          <div class="index">03</div>
          <span class="orange"></span>
          <div class="title">时尚活动与发布</div>
          <p class="title_english">Fashion events</p>
          <ul class="content">
            <li>10.29日上午，知识产权出版社原创认证保护平台刘睿、李</li>
            <li>静、彭梅在武汉市江岸区黄浦创立方园区参加了由武汉市江岸</li>
            <li>区科技局组织的武汉原创认证保护江岸分中心宣传会，对原创</li>
            <li>认证保护平台落户江岸进行调研与探讨。</li>
          </ul>
          <a href="javascript:void(0);" class="look_more">查看更多</a>
          <span class="small_orange"></span>

          <div class="pic_box">
            <div class="pic te relative">
              <MaskContainer/>
              <img src="../../assets/index/ssz4.jpg" alt>
            </div>
            <div class="pic relative">
              <MaskContainer/>
              <img src="../../assets/index/ssz5.jpg" alt>
            </div>
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
</style>
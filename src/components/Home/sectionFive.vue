<template>
  <div>
    <h3 id="anchor5">
      <div class="five">
        <div class="gy_index">05</div>
        <div class="gy_orange"></div>
        <div class="gy_title">供应链</div>
        <div class="gy_title_eg">supply chain</div>
        <div class="gy_content">
          <div class="gy_content_left">
            <div class="box">
              <div class="pic te_1 relative">
                <MaskContainer/>
                <img src="../../assets/index/t1.jpg" alt>
              </div>
              <div class="pic te_2 relative">
                <MaskContainer/>
                <img src="../../assets/index/t2.jpg" alt>
              </div>
            </div>
            <div class="box">
              <div class="pic te_3 relative">
                <MaskContainer/>
                <img src="../../assets/index/t4.jpg" alt>
              </div>
              <div class="pic te_4 relative">
                <MaskContainer/>
                <img src="../../assets/index/t3.jpg" alt>
              </div>
            </div>
          </div>
          <div class="gy_content_middle pic relative">
            <MaskContainer/>
            <img src="../../assets/index/t5.jpg" alt>
          </div>
          <div class="gy_content_right pic relative">
            <MaskContainer/>
            <img src="../../assets/index/t6.jpg" alt>
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
   .five{
    margin-bottom:150px;
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
    .gy_content{
      background:#e8e8e8;
      overflow: hidden;
      padding:40px 0;
      .gy_content_left{
        width:44%;
        float:left;
        .box{
          overflow: hidden;
        }
        .pic{
          float:left;
          margin-bottom:20px;
          position: relative;
          img{
            width:100%;
          }
          &.te_1{
            width:36.5%;
            float:left;
          }
          &.te_2{
            width:60.5%;
            float:right;
          }
          &.te_3{
            width:60.5%;

            float:left;
          }
          &.te_4{
            width:36.5%;
            float:right;

          }
        }
      }
      .gy_content_middle{
        float:left;
        width:21%;

          img{
            width:100%;
          }
        margin-left:1.5%;
      }
      .gy_content_right{
        width:32%;
        float:right;

          img{
            width:100%;
          }

      }
    }

  }
</style>
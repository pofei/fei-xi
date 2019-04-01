<template>
  <div class="section_two_container">
    <h3 id="anchor2">
      <a-carousel effect="fade">
        <a slot="customPaging" slot-scope="props" class="anchor2-dot">
            <span>{{getTitle(props.i)}}</span>
            <span class="line"></span>
        </a>
        <div class="two" v-for="(item, i) in titleList" :key="i">
            <div class="designer relative">
              <img src="../../assets/index/gx021.jpg" class="designer_img_left" alt>
            </div>
            <img src="../../assets/index/gx022.jpg" class="designer_img_right" alt>
            <div class="middle_content">
              <h4>设计师孵化</h4>
              <h5>Designer incubation</h5>
              <p>红T时尚创意街区重视行业顶尖人才、企业的引入，通过专业化服务、市场化推广、平台化运营，签约设计师品牌集合店、金顶奖设计师和全国十佳设计师和独立设计师工作室。目前签约入驻的有金顶设计师潘怡良、荷兰籍设计界怪才胡社光，品牌设计师罗钒溪，珠宝设计师lisa等。</p>
              <a href="javascript:void(0);" class="look_more">查看更多</a>
              <span class="small_orange"></span>
            </div>
        </div>
      </a-carousel>
    </h3>
  </div>
</template>

<script>
// import MaskContainer from '../../components/Home/mask.vue';

export default {
  data() {
    return {
      titleList: ["标题1", "标题2", "标题3", "标题4"]
    };
  },
  methods: {
    getTitle(i) {
      return this.titleList[i];
    }
  },
  components: {
    // MaskContainer
  }
};
</script>

<style scoped lang="less">


.relative {
  position: relative;
  overflow: hidden;
}
.section_two_container {
  margin-bottom: 287px;
  /deep/.slick-dots {
    top: 50%;
    margin: 9% 0 0px;
    .anchor2-dot {
        display: inline-block;
        padding: 0 5px;
        text-align: left;
        color: #000;
        overflow: hidden;
        .line {
            width: 0px;
            height: 1px;
            display: inline-block;
            margin-left: 5px;
            vertical-align: middle;
            transition: all .6s;
            background-color: #000;
        }
    }
    /deep/.slick-active {
        position: relative;
        text-align: left;
        .anchor2-dot {
            color: red;
            .line {
                width: 50px;
                background-color: red;
            }
        }
    }
}
}
.same_content {
  width: 1200px;
  overflow: hidden;
  margin: 0 auto;
  .orange {
    display: block;
    width: 8px;
    height: 50px;
    background: #cfa972;
  }
  .small_orange {
    display: block;
    width: 48px;
    height: 3px;
    background: #cfa972;
  }
  .title {
    font-size: 30px;
    color: #000;
  }
  .title_english {
    font-size: 18px;
    color: #000;
  }
  .content {
    font-size: 16px;
    color: #0d0d0d;
    line-height: 30px;
  }
  .look_more {
    font-size: 16px;
    font-weight: bold;
    color: #333;
  }
  &.content_right {
    position: relative;
    text-align: right;
    .orange {
      margin-left: 590px;
    }
    .small_orange {
      margin-left: 552px;
    }
  }
  .son {
    float: left;
    width: 600px;
  }
  .pic_box {
    margin-top: 57px;
    width: 100%;
    overflow: hidden;
    .pic {
      width: 288px;
      float: left;
      position: relative;
      &.te {
        margin-right: 24px;
      }
      img {
        width: 100%;
        height: 196px;
      }
    }
  }
  .son_right {
    width: 580px;
    margin: 0 10px;
    img {
      width: 100%;
    }
  }
}
.two {
  min-width: 1200px;
  overflow: hidden;
  position: relative;
  background: url("../../assets/index/gx02bj.jpg") right top no-repeat;
  .designer {
    width: 50%;
    float: left;
    height: 100%;
    position: relative;
    .designer_img_left {
      width: 100%;
    }
  }
  .designer_img_right {
    width: 28%;
    position: absolute;
    left: 68%;
    top: 53%;
    transform: translateY(-50%);
  }
}
.middle_content {
  position: absolute;
  width: 36%;
  height: 320px;
  margin-top: -140px;
  left: 32%;
  top: 50%;
  background: #fff;
  padding: 30px;
  z-index: 3;
  h4 {
    font-family: "仿宋";
    font-size: 22px;
    line-height: 1.5;
    clear: both;
    font-weight: bold;
  }
  h5 {
    font-family: "Georgia";
    font-size: 16px;
    text-transform: uppercase;
    letter-spacing: 4px;
  }
  p {
    height: 110px;
    overflow: hidden;
    line-height: 20px;
    margin-bottom: 10px;
    font-size: 14px;
    color: #000;
  }
  .look_more {
    font-size: 16px;
    float: right;
    color: #000;
    padding-bottom: 5px;
    border-bottom: 3px solid #c8a384;
  }
}
</style>
<template>
  <div class="activity">
    <div class="activity-banner">
      <div class="container">
        <h1>中国国际品牌服装服饰交易会</h1>
        <p class="title">Fashion China SHOW</p>
        <p class="time">2019年04月08日 下午 14：00</p>
        <a-button class="btn" type="primary">立即预定</a-button>
      </div>
    </div>
    <div class="container">
      <div class="tabs">
        <Tab :list='tabsName.time'></Tab>
        <Tab :list='tabsName.interest'></Tab>
        <Tab :list='tabsName.city'></Tab>
      </div>
      <a-divider />
      <div class="cards">
        <a-row type="flex" justify="start">
          <a-col class="cards-in" :xs="24" :sm="24" :md="12" :lg="8" :xl="8" :key="item" v-for="item in arr">
            <div class="card" >
              <h3 >2019广州白马服装采购节（春夏）</h3>
              <p class="time">2019-03-05</p>
              <img class="pic" src="../assets/images/activity/item.jpg" alt="">
              <p class="address">广东省深圳市福田区深圳会展中心</p>
              <a-divider />
            </div>
          </a-col>
        </a-row>
      </div>
      <div class="more">
          <span>更多 > ></span>
      </div>
    </div>
  </div>
</template>

<script>
import Tab from '@/components/Tab/Tab'
const tabsName = {
  time: { 'title': '时间', 'list': ['全部', '今天', '明天', '本周', '本周末', '本月'] },
  interest: { 'title': '兴趣', 'list': ['全部', '会议', '展览', '论坛', '课程', '讲座', '沙龙', '聚会', '发布会', '赛事', '分享会', '公开课', '其他'] },
  city: { 'title': '城市', 'list': ['全部', '武汉', '上海', '广州', '深圳', '东莞', '青岛', '成都', '杭州', '南京', '郑州', '宁波', '石家庄', '株洲'] }
}
export default {
  name: 'activity',
  data () {
    return {
      tabsName,
      arr: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]
    }
  },
  components: {
    Tab
  }
}
</script>

<style lang="less" scoped>
.activity {
  .activity-banner {
    width: 100%;
    height: 566px;
    background-image: url(../assets/images/activity/activity_banner.jpg);
    .container{
      text-align: center;
      color: #fff;
      padding-top: 140px;
      h1{
        font-size:54px;
        font-weight: normal;
        color: #fff;
      }
      .title{
        font-size:48px;
        line-height:50px;
        margin-bottom: 30px;
      }
      .time{
        font-size: 30px;
        line-height: 28px;
      }
      .btn{
        width:186px;
        height:40px;
        background:rgba(254,254,254,1);
        font-size:24px;
        font-weight:normal;
        letter-spacing: 0.7px;
        color:rgba(78,139,248,1);
        line-height:40px;
        border: 0 none;
        outline: none;
        cursor: pointer;
      }
    }

  }
  .container{
    width: 1318px;
    margin: 0 auto;
    .tabs{
      margin-top: 36px;
    }
    .cards{
      padding-top: 30px;
      .card{
        h3{
          font-size: 18px;
          margin-bottom: 3px;
        }
        .time{
          background: url(../assets/images/activity/time.png) no-repeat left center;
          padding-left: 36px;
          margin-bottom: 10px;
          line-height: 20px;
        }
        .pic{
          width: 419px;
          height: 206px;
        }
        .address{
          font-size: 18px;
          margin-top: 15px;
        }
        .divider{
          display: none;
        }
      }
    }
    .more{
      width: 1200px;
      height: 80px;
      line-height: 80px;
      margin: 0 auto;
      text-align: center;
      font-size:24px;
      cursor: pointer;
      margin-bottom: 20px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
      color: #40434a;
      margin-top: 20px;

    }
  }
}

</style>

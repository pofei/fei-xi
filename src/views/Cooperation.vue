<template>
  <div class="cooperation">
    <div class="cooperation-banner"></div>
    <div class="container">
      <div class="tabs">
        <Tab :list='tabsName.time'></Tab>
        <Tab :list='tabsName.interest'></Tab>
        <Tab :list='tabsName.city'></Tab>
      </div>
      <a-divider />
      <div class="cards">
        <a-row type="flex" justify="space-between">
            <div class="card" :key="item" v-for="item in arr" >
              <h3>吴江市鑫泓润实业有限公司</h3>
              <img class="pic" src="../assets/images/cooperation/item.jpg" alt="">
            </div>
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
  name: 'cooperation',
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
.cooperation {
  .cooperation-banner {
    width: 100%;
    height: 566px;
    background-image: url(../assets/images/cooperation/co_banner.jpg);
  }
  .container{
    max-width: 1318px;
    margin: 0 auto;
    .tabs{
      margin-top: 36px;
    }
    .cards{
      padding-top: 30px;
      .card{
        h3{
          font-size: 28px;
        }
        .pic{
          margin-bottom: 73px;
          width: 419px;
          height: 206px;
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
      margin-top: 20px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
      color: #40434a;
    }
  }
}

</style>

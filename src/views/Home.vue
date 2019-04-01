<template>
  <div class="home">
    <Carousel/>
    <SliderTab/>
    <AnchorList/>
    <SecitionOne />
    <SecitionTwo />
    <SecitionThree />
    <SecitionFour />
    <SecitionFive />
    <SecitionSix />
    <SectionSeven />
  </div>
</template>

<script>
import Carousel from '../components/Home/crausel.vue';
import SliderTab from '../components/Home/sliderTab.vue';
import AnchorList from '../components/Home/anchorList.vue';
import SecitionOne from '../components/Home/sectionOne.vue';
import SecitionTwo from '../components/Home/sectionTwo.vue';
import SecitionThree from '../components/Home/sectionThree.vue';
import SecitionFour from '../components/Home/sectionFour.vue';
import SecitionFive from '../components/Home/sectionFive.vue';
import SecitionSix from '../components/Home/sectionSix.vue';
import SectionSeven from '../components/Home/sectionSeven.vue';
export default {
  name: 'home',
  components: {
    Carousel,
    SliderTab,
    AnchorList,
    SecitionOne,
    SecitionTwo,
    SecitionThree,
    SecitionFour,
    SecitionFive,
    SecitionSix,
    SectionSeven
  }
}
</script>

<style scoped lang="less">
.home {
  width: 100%;
  text-align: left;
}

.index {
  font-size: 30px;
  color: #000;
}

</style>

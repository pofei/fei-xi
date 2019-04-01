<template>
    <div class="banner-container">
        <a-carousel arrows effect="fade">
            <div
            slot="prevArrow" 
            class="custom-slick-arrow"
            style="left: 10px;zIndex: 1"
            >
                <a-icon type="left-circle" />
            </div>
            <div
            slot="nextArrow"
            class="custom-slick-arrow"
            style="right: 10px"
            >
                <a-icon type="right-circle" />
            </div>
            <div class="te"><img class="carousel-img" src="../../assets/index/banner0.jpg" alt=""></div>
            <div class="te"><img class="carousel-img" src="../../assets/index/banner3.jpg" alt=""></div>
            <div class="te"><img class="carousel-img" src="../../assets/index/banner4.jpg" alt=""></div>
        </a-carousel>
    </div>
</template>

<script>
    export default {
    }
</script>

<style scoped lang="less">
    .banner-container {
      width: 100%;
       .te{
           width:100%;
           height:880px;
           position: relative;
           .carousel-img {
               height:100%;
               position: relative;
               left: 50%;
               transform: translateX(-50%);
               display: block;
           }
       }

      .custom-slick-arrow {
        width: 50px;
        height: 50px;
        font-size: 50px;
        color: #fff;
        background-color: rgba(31,45,61,.11);
        opacity: 0.3;
        &::before {
          display: none;
        }
        &:hover {
          opacity: 0.5;
        }
      }
    }
</style>
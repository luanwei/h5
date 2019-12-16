<template>
  <div class="view">
    <div class="swiper-container">
      <div class="swiper-wrapper">
        <div class="swiper-slide">
          <img src="../../assets/image/map-1.jpg" alt="">
        </div>
        <div class="swiper-slide" >
          <img src="../../assets/image/map-2.jpg" alt="">
        </div>
      </div>
    </div>
    <div class="top">
      <!--      <img class="map-1" src="../../assets/image/map-1.jpg">-->
      <!--      <span>重庆市服务网点全覆盖</span>-->
      <!--      <img class="map-2" src="../../assets/image/map-2.jpg">-->
      <img class="jq-1" src="../../assets/image/jq-1.jpg">
      <img class="jq-2" src="../../assets/image/jq-2.jpg">
      <img class="jq-3" src="../../assets/image/jq-3.jpg">
    </div>
    <div :class="{'run-animation':isShow1 }" class="l-l animation-container animation-fade-right">
      <span>◆</span> 重庆监管机构评级：
      <span>AA</span>
    </div>
    <div :class="{'run-animation':isShow2 }" class="l-c animation-container animation-fade-left">
      ——行业排名第三
    </div>
    <div :class="{'run-animation':isShow3 }" class="l-l animation-container animation-fade-right">
      <span>◆</span>重庆赔得最快的保险公司
    </div>
    <div :class="{'run-animation':isShow4 }" class="l-c animation-container animation-fade-left">
      <span>——</span>
      <div>报案支付时效快于同业5天，万元以下小额案件快于同业1天</div>
    </div>
    <div :class="{'run-animation':isShow5 }" class="l-l animation-container animation-fade-right">
      <span>◆</span>重庆唯一保持零投诉的保险公司
    </div>

  </div>
</template>

<script>
import Swiper from 'swiper'
export default {
  components: {},
  data() {
    return {
      isShow1: false,
      isShow2: false,
      isShow3: false,
      isShow4: false,
      isShow5: false
    }
  },
  created() {
  },
  mounted: function() {
    var mySwiper = new Swiper('.swiper-container', {
      autoplay: true,
      loop: true
    })
    this.showAnimation()
  },

  methods: {
    showAnimation() {
      setTimeout(() => {
        this.isShow1 = true
      }, 700)
      setTimeout(() => {
        this.isShow2 = true
      }, 900)
      setTimeout(() => {
        this.isShow3 = true
      }, 1100)
      setTimeout(() => {
        this.isShow4 = true
      }, 1300)
      setTimeout(() => {
        this.isShow5 = true
      }, 1500)
    }
  }
}
</script>
<style lang="scss" scoped>
.top {
  display: block;
  position: relative;
  height: 29vw;
  z-index: 1;
  display: flex;
  align-items: center;
  justify-content: space-around;
  width: 75%;
  margin: 0 12.5%;
  /* margin-top: -10vw; */
  .map-1 {
    position: absolute;
    top: 3.2vw;
    left: 12.2vw;
    width: 34.4667vw;
    height: 29.33vw;
    z-index: 2;
  }

  .map-2 {
    position: absolute;
    top: 5.2vw;
    left: 53.2vw;
    width: 37.6vw;
    height: 33.6vw;
    z-index: 2;
  }
  span {
    position: absolute;
    top: 3.2vw;
    left: 52.2vw;
    color: red;
    font-size: 3.2vw;
    z-index: 3;
  }
  .jq-1 {
    /*position: absolute;
    top: 5vw;
    left: 6.2vw;*/
    /* width: 11.73vw; */
    width: auto;
    height: 27vw;
  }
  .jq-2 {
   /* position: absolute;
    top: 5vw;
    left: 21.2vw;*/
    /*  width: 9.1333vw; */
    width: auto;
    height: 27vw;
  }
  .jq-3 {
    /*position: absolute;
    top: 5vw;
    left: 35.2vw;*/
    /* width: 9.1333vw; */
    width: auto;
    height: 27vw;
  }
}

.l-l {
  display: flex;
  align-items: center;
  justify-content: flex-start;
  height: 8vw;
  padding-left: 12vw;
  font-size: 4.5vw;
  color: #006666;
  margin-top: 2vh;
  span {
    margin-right: 1.3vw;
  }
   :nth-of-type(2) {
    color: red;
    font-size: 4vw;
    font-weight: 600;
  }
}

.l-c {
  display: flex;
  line-height: 6vw;
  /* color: #006666; */
  color: #404040;
  justify-content: flex-start;
  font-size: 3.9vw;
  padding: 1vw 5.333vw 1vw 15vw
}

.swiper-slide {
  position: relative;
  width: 100%;
  height: 57vw;
  display: flex;
  justify-content: center;
  align-items: center;
  padding-top: 3.2vw;
  padding-bottom: 1vw;
}

.swiper-container {
  
}

.swiper-slide img {
  height: 100%;
  width: auto;
}
</style>

<template>
  <div class="view">
    <img class="t-banner" src="../../assets/image/yyzz_t.jpg">
    <div :class="{'run-animation':isShow1 }" class="l-red animation-container animation-fade-right" ><i>★</i> 2010年获评：企业集团发展金融<span>典型成功案例</span></div>
    <div :class="{'run-animation':isShow2 }" class="l-red animation-container animation-fade-right"><i>★</i>2012年位列财险公司<span>盈利能力第一位</span></div>
    <div :class="{'run-animation':isShow3 }" class="l-right animation-container animation-fade-left"> ——《中国保险业竞争力报告》</div>
    <div :class="{'run-animation':isShow4 }" class="l-red animation-container animation-fade-right"><i>★</i> 2013年位列中<span>国保险业 综合竞争力第三位</span></div>
    <div :class="{'run-animation':isShow5 }" class="l-right animation-container animation-fade-left"> ——《中国保险业竞争力报告》</div>
    <div :class="{'run-animation':isShow6 }" class="l-red animation-container animation-fade-right"><i>★</i> 2014年获评<span>中国价值成长十佳保险公司</span></div>
    <div :class="{'run-animation':isShow7 }" class="l-red animation-container animation-fade-right"><i>★</i> 公司研发的系列电网产品，被确定为<span>行业标准</span></div>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      isShow1: false,
      isShow2: false,
      isShow3: false,
      isShow4: false,
      isShow5: false,
      isShow6: false,
      isShow7: false
    }
  },
  created() {
  },
  mounted: function() {
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
      setTimeout(() => {
        this.isShow6 = true
      }, 1700)
      setTimeout(() => {
        this.isShow7 = true
      }, 2100)
    }
  }
}
</script>
<style lang="scss" scoped>
  .t-banner {
    display: block;
    width: 100%;
    height: 55vw;
    margin-bottom: 8vw;
  }
  .l-red{
    width: 100%;
    font-size: 4vw;
    height: 6vw;
    display: flex;
    align-items: center;
    justify-content: flex-start;
    padding: 5.3vw;
    i{
      font-style: normal;
      color:red;
      margin-right: 3px;
    }
    span{
      color: red;
      font-size: 4.5vw;
      font-weight: 600;
    }
  }
  .l-right{
    height: 6vw;
    display: flex;
    align-items: center;
    justify-content: flex-end;
    font-size: 4vw;
    text-align: right;
    padding: 5.3vw;
  }
</style>

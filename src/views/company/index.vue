<template>
  <div class="view">
    <img class="t-banner" src="../../assets/image/company_t.jpg" />
    <div class="title">我们是——</div>
    <div :class="{'run-animation':isShow }" class="slogan animation-container animation-fade-right">
      国家电网自己的财产保险公司
      <br />精心服务电力职工的保险公司
    </div>
    <div
      :class="{'run-animation':isShow1 }"
      class="describe animation-container animation-fade-right"
    >
      总公司成立于2008年9月
      <br />总部设在北京
      <br />重庆分公司成立于2016年9月
      <br />位于市电力公司昆亚大厦7-8楼
      <br />
    </div>

    <div :class="{'run-animation':isShow2 }" class="b-table animation-container animation-fade-up">
      <div @click="goPage('yyzz')">
        <img src="@/assets/image/d1.png" alt />
        <span>优质服务</span>
      </div>
      <div @click="goPage('fwpz')">
        <img src="@/assets/image/d2.png" alt /><span>服务品质</span></div>
      <div @click="goPage('smrw')">
        <img src="@/assets/image/d3.png" alt /><span>使命服务</span></div>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      isShow: false,
      isShow1: false,
      isShow2: false
    };
  },
  created() {},
  mounted: function() {
    this.showAnimation();
  },
  methods: {
    goPage(type) {
      switch (type) {
        case "yyzz":
          this.$router.push({ path: "/yyzz" });
          break;
        case "fwpz":
          this.$router.push({ path: "/fwpz" });
          break;
        case "smrw":
          this.$router.push({ path: "/smrw" });
          break;
      }
    },
    showAnimation() {
      setTimeout(() => {
        this.isShow = true;
      }, 700);
      setTimeout(() => {
        this.isShow1 = true;
      }, 900);
      setTimeout(() => {
        this.isShow2 = true;
      }, 1000);
    }
  }
};
</script>
<style lang="scss" scoped>
.t-banner {
  display: block;
  width: 100%;
  height: 55vw;
}

.b-table {
  position: absolute;
  bottom: 0;
  right: 0;
  left: 0;
  width: 100%;
  height: 13.4vw;
  display: flex;
  justify-content: center;
  align-items: center;
  border-top: 1px solid #D5D5D5;

  div {
    flex: 1;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    height: 13.4vw;
    color:rgba(0,102,102,0.8);
   /*  border-right: 1px solid #040404; */
    font-size: 2.5vw;
    font-weight: 600;

    img{
      width: 7vw;
    }
  }

  :nth-last-of-type(1) {
    border-right: none;
  }
}

.title {
  font-size: 4.53vw;
  line-height: 6vw;
  color: #006666;
  padding: 0 5.3vw;
  text-align: left;
  margin: 4vw;
}

.slogan {
  text-align: center;
  color: #006666;
  font-size: 5vw;
  font-weight: 600;
  line-height: 2;
}

.describe {
  width: 60%;
  margin-top: 4vh;
  margin-right: 7%;
  margin-left: 30%;
  text-align: left;
  color: #040404;
  font-size: 4.1vw;
  line-height: 1.8;
  letter-spacing: 1px;
}
</style>

<template>
  <div class="view">
    <img class="t-banner" src="@/assets/image/service.jpg" />
    <div class="list-box">
      <ul class="list">
        <li @click="goPage('zdfw')">
          <div class="bk-s1">
            <img src="@/assets/image/s_1.png" />
          </div>
          <span>专设驻</span>
          <span>点服务</span>
        </li>
        <li @click="goPage('cpfw')">
          <div class="bk-s2">
            <img src="@/assets/image/s_2.png" />
          </div>
          <span>专属产</span>
          <span>品服务</span>
        </li>
        <li @click="goPage('lptd')">
          <div class="bk-s3">
            <img src="@/assets/image/s_3.png" />
          </div>
          <span>专属理</span>
          <span>赔通道</span>
        </li>
        <li @click="goPage('dljy')">
          <div class="bk-s4">
            <img src="@/assets/image/s_4.png" />
          </div>
          <span>全国道</span>
          <span>路救援</span>
        </li>
        <li @click="goPage('jsfw')">
          <div class="bk-s5">
            <img src="@/assets/image/s_5.png" />
          </div>
          <span>代办检</span>
          <span>审服务</span>
        </li>
        <li @click="goPage('ajfw')">
          <div class="bk-s6">
            <img src="@/assets/image/s_6.png" />
          </div>
          <span>定期安</span>
          <span>检服务</span>
        </li>
        <li @click="goPage('cgj')">
          <div class="bk-s7">
            <img src="@/assets/image/s_7.png" />
          </div>
          <span>"车管家"</span>
          <span>服务</span>
        </li>
        <li @click="goPage('zlfw')">
          <div class="bk-s8">
            <img src="@/assets/image/s_8.png" />
          </div>
          <span>索赔助</span>
          <span>理服务</span>
        </li>
      </ul>
    </div>
    <div class="content-box margin-h-10">
      <h5>工会协同</h5>
      <p
        class="font-size-16 font-family-s color-black-a margin-top-8"
      >在各级工会设立“服务监督员”，维权监督，让您更安心、更放心。</p>
      <p
        class="font-size-16 font-family-s color-black-a margin-top-8"
      >共同打造电力职工独享的服务优势与价值优势，让特别优待惠及每一位职工。</p>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {};
  },
  created() {},
  mounted: function() {},

  methods: {
    goPage(type) {
      if (type == "zlfw") {
        this.$router.push({ path: "/spzlfw"});
      }else if (type == "cgj") {
        this.$router.push({ path: "/cgjfw"});
      }else{
this.$router.push({ path: "/detail", query: { type: type } });
      }
      
    }
  }
};
</script>
<style lang="scss" scoped>
.t-banner {
  display: block;
  width: 80%;
  height: auto;
  margin-left: 10%;
}

.list-box {
  width: 90%;
  margin: -10% 5% 0% 5%;
  display: inline-block;
  font-size: 1.8rem;
  color: #006666;
}

.list li {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  flex-wrap:wrap;
  list-style: none;
  width:24%;
  height: 23vw;
  float: left;
  text-align: center;
  margin: 0.8rem 0.5%;
  /*border: 1px solid rgba(0, 102, 102, 0.5);*/
  padding: 0.6rem 0;
  border-radius: 0.6rem;
  cursor: pointer;
  margin-top: 3.2vw;
}
.list li div {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 12vw;
  height: 12vw;
  border-radius: 4.6vw;
}
.list li div img {
  width: 6vw;
  height: 6vw;
}
.list li span {
  font-size: 3.45vw;
    padding: 0 1vw;
}
.content-box h5 {
  font-size: 2rem;
}

.content-box p {
  padding-left: 3rem;
}

.bk-s1 {
  background-color: #87ceeb;
}

.bk-s2 {
  background-color: #d2691e;
}

.bk-s3 {
  background-color: #dda0dd;
}

.bk-s4 {
  background-color: #ff4500;
}

.bk-s5 {
  background-color: #a52a2a;
}

.bk-s6 {
  background-color: #ff8c00;
}

.bk-s7 {
  background-color: #ffd700;
}

.bk-s8 {
  background-color: #1e90ff;
}
</style>

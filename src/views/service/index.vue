<template>
  <div class="view">
    <img class="t-banner" src="@/assets/image/service.jpg" />
    <div class="list-box">
      <ul class="list">
        <li @click="goPage('zdfw')">专设驻点服务</li>
        <li @click="goPage('cpfw')">专属产品服务</li>
        <li @click="goPage('lptd')">专属理赔通道</li>
        <li @click="goPage('dljy')">全国道路救援</li>
        <li @click="goPage('jsfw')">代办检审服务</li>
        <li @click="goPage('ajfw')">定期安检服务</li>
        <li @click="goPage('cgj')">“车管家”服务</li>
        <li @click="goPage('zlfw')">索赔助理服务</li>
      </ul>
    </div>
    <div class="content-box margin-h-10">
      <h5>工会协同</h5>
      <p class="font-size-16 font-family-s color-black-a margin-top-8">在各级工会设立“服务监督员”，维权监督，让您更安心、更放心。</p>
      <p class="font-size-16 font-family-s color-black-a margin-top-8">共同打造电力职工独享的服务优势与价值优势，让特别优待惠及每一位职工。</p>
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
      this.$router.push({ path: "/detail", query: { type: type } });
    }
  }
};
</script>
<style lang="scss" scoped>
.t-banner {
  display: block;
  width: 80%;
  height:auto;
  margin-left: 10%;
}

.list-box {
  width: 80%;
  margin: -10% 10% 0% 10%;
  display: inline-block;
  font-size: 1.8rem;
  color: #006666;
}

.list li {
  list-style: none;
  width: 45%;
  float: left;
  text-align: center;
  margin: 0.8rem 2.5%;
  border: 1px solid rgba(0, 102, 102, 0.5);
  padding: 0.6rem 0;
  border-radius: 0.6rem;
  cursor: pointer;
}

.content-box h5{
  font-size: 1.8rem;
}
</style>

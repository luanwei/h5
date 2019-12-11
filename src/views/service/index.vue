<template>
  <div class="view">
    <img class="t-banner" src="@/assets/image/service.jpg" />
    <div class="list-box">
      <ul class="list">
        <li>专设驻点服务</li>
        <li>专属产品服务</li>
        <li>专属理赔通道</li>
        <li>全国道路救援</li>
        <li>代办检审服务</li>
        <li>定期安检服务</li>
        <li>“车管家”服务</li>
        <li>索赔助理服务</li>
      </ul>
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

  methods: {}
};
</script>
<style lang="scss" scoped>
.t-banner {
  display: block;
  width: 100%;
  height: 33%;
}

.list-box {
  margin: 2% 10%;
  display: inline-block;
  font-size: 1.8rem;
  color: #006666;
}

.list li {
  list-style: none;
  width: 50%;
  float: left;
  text-align: center;
  margin: 1rem 0;
  border: 1px solid;
  padding: 0.6rem 0;
}
</style>

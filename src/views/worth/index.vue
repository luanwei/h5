<template>
  <div class="view">
    <div class="img-box">
      <img src="@/assets/image/worth.png" />
    </div>
    <div class="wrap1">
      <p>在别的公司，您是一个普通的车险客户</p>
      <p>在国网英大，您就是我们贴心维护的“使命VIP”!</p>
    </div>
    <div class="wrap2 content-box">
      <h5>各项免费活动贯穿全年</h5>
      <p>为期一月的“315 客户节”活动、“泰和迎春”专题服务活动、“泰和金秋”专题服务活动、“零赔付”客户关爱活动</p>
      <h5>与德国 "伍尔特"深度合作</h5>
      <p>
        联合德国顶级养活品牌“伍尔特”引领科学保养，尊享
        高端特惠（承保职工 5.5 折，未承保职工 7.5 折）
      </p>
      <h5>与"途虎" 连锁店深度合作</h5>
      <p>
       联合“途虎养车”连锁店，提供特别优待或部分免费服务（推介集“红心”，换多重价值服务）
      </p>
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
.img-box {
  margin-bottom: 5%;
}
.img-box img {
  width: 60%;
  margin-left: -6%;
  margin-top: 4%;
}


.wrap1{
   position: absolute;
  width: 53%;
  right: 5%;
  top: 4%;
  color: #006666;
  font-size: 20px;
  font-weight: 700;
  letter-spacing: 2px;
}

.wrap1>p:nth-of-type(1){
  margin-bottom: 20px;
}

@keyframes show1 {
  0%{
    margin-bottom: 50px;
    
  }

  100%{
    margin-bottom: 20px;
    opacity: 1;
  }
}

.wrap2{
  position: absolute;
}
.t-banner {
  display: block;
  width: 100%;
  height: 32vw;
}
</style>

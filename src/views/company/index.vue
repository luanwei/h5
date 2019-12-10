<template>
  <div class="view">
    <img class="t-banner" src="../../assets/image/sy_t.jpg">
    <div></div>
    <div class="b-table">
      <div>优质服务</div>
      <div>服务品质</div>
      <div>使命服务</div>
    </div>
  </div>
</template>

<script>

  export default {
    components: {},
    data() {
      return {}
    },
    created() {
    },
    mounted: function () {

    },

    methods: {}
  }
</script>
<style lang="scss" scoped>
  .t-banner {
    display: block;
    width: 100%;
    height: 32vw;
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
    border-top: 1px solid #333333;

    div {
      flex: 1;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 13.4vw;
      border-right: 1px solid #333333;
      font-size: 4vw;
      font-weight: 600;
    }

    :nth-last-of-type(1) {
      border-right: none;
    }
  }
</style>

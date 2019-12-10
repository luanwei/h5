<template>
  <div class="view">
    <img class="t-banner" src="../../assets/image/sy_t.jpg">
    <div class="b-table">
      <div @click="goPage('yyzz')">优质服务</div>
      <div @click="goPage('fwpz')">服务品质</div>
      <div @click="goPage('smrw')">使命服务</div>
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
  mounted: function() {
  },
  methods: {
    goPage(type) {
      switch (type) {
        case 'yyzz':
          this.$router.push({ path: '/yyzz' })
          break
        case 'fwpz':
          this.$router.push({ path: '/fwpz' })
          break
        case 'smrw':
          this.$router.push({ path: '/smrw' })
          break
      }
    }
  }
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

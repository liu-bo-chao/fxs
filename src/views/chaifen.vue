<template>
  <div class="div">
    <div class="div4"></div>
    <div class="div4-1">
      <p class="div4-2">
        这里有一堆字，这里有一堆字，这里有一堆字，这里有一堆字，这里有一堆字，这里有一堆字，这里有一堆字，这里有一堆字，这里有一堆字，这里有一堆字，
      </p>
    </div>
    <div class="div4"></div>
    <div class="div5">
      <p class="div5-1">服务热线：400-9977-658</p>
      <van-tabs v-model="active">
        <van-tab title="触屏版"></van-tab>
        <van-tab title="电脑版"></van-tab>
        <van-tab title="关于我们"></van-tab>
        <van-tab title="联系我们"></van-tab>
      </van-tabs>
      <p class="pp">
        <img src="/imgs/2.png" alt="" />
        <span class="spanimgs"><img src="/imgs/3.png" alt="" /></span>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "",
  data() {
    return {};
  },
  mounted() {
  },
  methods: {},
  computed: {},
  watch: {},
};
</script>

<style lang="scss" scoped>
.div {
  width: 100%;
  height: 100%;
   
  background: #fff;
}
.div4 {
  width: 100%;
  height: 10px;
}
.div4-1{
    background: #fff;
    width: 100%;
    height: 130px;
}
.div4-2{
    margin: 0;
}
.pp {
  width: 100%;
  height: 100px;
  position: relative;
  background-color: rgba($color: #000000, $alpha: 0.7);
  img {
    margin-left: 30px;
    width: 80%;
    height: 100%;
  }
  .spanimgs {
    position: absolute;
    top: 0;
    left: -30px;
    img {
      width: 40px;
      height: 40px;
    }
  }
}
</style>

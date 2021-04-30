<template>
  <div class="divv">
    <!-- 头部 -->
    <div class="div">
      <div class="div1">
        <van-row>
          <van-col span="8">
              <img class="imggg" src="/imgs/ma.jpg" alt="">
          </van-col>
          <van-col span="14" class="spimg"
            ><img src="/imgs/rrm.png" alt="" />
            <p class="span1">
              关注房先森官方微信公众号<span class="span2">sirfang_com</span>
            </p>
          </van-col>
          <van-col span="2" class="span">X</van-col>
        </van-row>
      </div>
      <van-search
        v-model="value"
        show-action
        placeholder="请输入关键词"
        @search="onSearch"
      >
        <template #action>
          <van-button type="primary">主要按钮</van-button>
        </template>
      </van-search>
    </div>
    <!-- 流程 -->
    <div class="div2">
      <van-tabs v-model="activeName">
        <van-tab title="装修前" name="a">
          <!-- 装修前 -->
        </van-tab>
        <van-tab title="装修中" name="b">
          <!-- 装修中 -->
        </van-tab>
        <van-tab title="装修后" name="c">
          <!-- 装修后 -->
        </van-tab>
      </van-tabs>
      <van-grid>
        <van-grid-item icon="shop-o" text="收房验房" />
        <van-grid-item icon="records" text="收房预算" />
        <van-grid-item icon="balance-pay" text="装修风水" />
        <van-grid-item icon="edit" text="装修设计" />
      </van-grid>
      <van-button class="but" type="primary">主要按钮</van-button>
    </div>
    <div class="div3">
      <p class="zi"><span class="pspan">1</span> 为您推荐</p>
      <van-row class="row">
        <van-col span="8"><img class="img1" src="/imgs/1.jpg" alt="" /></van-col>
        <van-col span="16">
          开发商延期交房，业主如何维权呢?
          <br />
          <br />
          <br />
          <p class="p1">
            <van-icon name="clock-o" />
            2016-07-07
            <span class="pspan1"> <van-icon name="eye" />115</span>
          </p>
        </van-col>
      </van-row>
      <van-row class="row">
        <van-col span="8"><img class="img1" src="/imgs/1.jpg" alt="" /></van-col>
        <van-col span="16">
          开发商延期交房，业主如何维权呢?
          <br />
          <br />
          <br />
          <p class="p1">
            <van-icon name="clock-o" />
            2016-07-07
            <span class="pspan1"> <van-icon name="eye" />115</span>
          </p>
        </van-col>
      </van-row>
      <van-row class="row">
        <van-col span="8"><img class="img1" src="/imgs/1.jpg" alt="" /></van-col>
        <van-col span="16">
          开发商延期交房，业主如何维权呢?
          <br />
          <br />
          <br />
          <p class="p1">
            <van-icon name="clock-o" />
            2016-07-07
            <span class="pspan1"> <van-icon name="eye" />115</span>
          </p>
        </van-col>
      </van-row>
      <van-row class="row">
        <van-col span="8"><img class="img1" src="/imgs/1.jpg" alt="" /></van-col>
        <van-col span="16">
          开发商延期交房，业主如何维权呢?
          <br />
          <br />
          <br />
          <p class="p1">
            <van-icon name="clock-o" />
            2016-07-07
            <span class="pspan1"> <van-icon name="eye" />115</span>
          </p>
        </van-col>
      </van-row>
      <van-row class="row">
        <van-col span="8"><img class="img1" src="/imgs/1.jpg" alt="" /></van-col>
        <van-col span="16">
          开发商延期交房，业主如何维权呢?
          <br />
          <br />
          <br />
          <p class="p1">
            <van-icon name="clock-o" />
            2016-07-07
            <span class="pspan1"> <van-icon name="eye" />115</span>
          </p>
        </van-col>
      </van-row>
      <van-button plain type="primary" class="but"
        >换一换<van-icon name="replay"
      /></van-button>
    </div>
  <chaifen/>
    <!-- <div class="div4"></div>
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
          <span class="spanimgs"><img src="/imgs/3.png" alt=""></span>
          </p>
    </div> -->
  </div>
</template>

<script>
import chaifen from './chaifen'
export default {
  name: "",
  components:{chaifen},
  data() {
    return {
      activeName: "a",
    };
  },
  mounted() {
    //this.axios.get('/').then((res) => {
    //this.result = res.result;
    //});
  },
  methods: {},
  computed: {},
  watch: {},
};
</script>

<style lang="scss" scoped>
* {
  margin: 0;
  padding: 0;
}
.divv {
  width: 100%;
  height: 100%;
  background: #f0f0f0;
}
.div {
  width: 100%;
  height: 150px;
  background: #f0f0f0;
}
.imggg{
    width: 80%;
    height: 85px;
    margin-left: 10px;
}
.div1 {
  width: 100%;
  height: 90px;
  background: aquamarine;
  .span1 {
    padding: 10px 2px;
    border: 1px solid;
    border-radius: 20px;

    font-size: 12px;
    .span2 {
      color: gold;
    }
  }
}
.div2 {
  width: 100%;
  height: 190px;
  background: #f0f0f0;
}
.spimg {
  padding-top: 10px;
  img {
    width: 80%;
    margin-bottom: 10px;
  }
}
.span {
  padding-left: 20px;
}
.van-search {
  padding: 0 10px;
}
.but {
  width: 100%;
  color: green;
  font-weight: 700;
  margin: 10px 0;
  font-size: 20px;
  background: #fff;
  border: 1px solid green;
}
.div3 {
  width: 100%;
  background: #fff;
  .zi {
    font-size: 20px;
    font-weight: 700;

    .pspan {
      height: 20px;
      background: green;
      color: green;
    }
  }
  .row {
    width: 100%;
    height: 100px;
    padding: 10px 0;
    font-size: 16px;
    border-bottom: 1px solid grey;
    .p1 {
      font-size: 12px;

      color: grey;
    }
    .img1 {
      width: 80%;
      height: 100px;
    }
    .pspan1 {
      padding: 0 20px;
    }
  }
}

// .div4 {
//   width: 100%;
//   height: 10px;
//   background: #f0f0f0;
// }
// .div4-1 {
//   width: 100%;
//   background: #fff;
//   .div4-2 {
//     padding: 10px;
//   }
// }
// .div5-1 {
//   width: 100%;
//   text-align: center;
//   margin: 10px;
// }
// .pp{
//      position: relative;
//     background-color: rgba($color: #000000, $alpha: 0.8);
//     img{
//         width: 80%;
//         margin: 10px 40px 0;
   

//     }
//     .spanimgs{
//         width: 40px;
//         height: 40px;
//         position: absolute;
//         left: -40px;
//         top: -10px;
//         img{
//             width: 40px;
//             height: 40px;
//         }
//     }
// }
</style>

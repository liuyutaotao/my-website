<template>
  <div class="home">
    <div class="info">
      <p>我们正在打造世界领先的</p>
      <h1>电力检测解决方案及</h1>
      <h1>电力监测设备</h1>
    </div>
    <!-- <img alt="Vue logo" src="../assets/logo.png" /> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <el-row
      type="flex"
      class="row-lb"
      justify="space-around"
    >
      <el-col :span="7">
        <!-- <el-carousel height="200px">
          <el-carousel-item
            v-for="item in 4"
            :key="item"
          >
            <h3 class="small">{{ item }}</h3>
          </el-carousel-item>
        </el-carousel> -->
        <el-carousel
          :interval="3000"
          height="200px"
        >
          <el-carousel-item>
            <img src="../assets/1.jpg">
          </el-carousel-item>
          <el-carousel-item>
            <img src="../assets/2.jpg">
          </el-carousel-item>
          <el-carousel-item>
            <img src="../assets/3.jpg">
          </el-carousel-item>
          <el-carousel-item>
            <img src="../assets/4.jpg">
          </el-carousel-item>
        </el-carousel>
      </el-col>
      <el-col :span="7">
        <el-carousel
          :interval="3000"
          height="200px"
        >
          <el-carousel-item>
            <img src="../assets/5.jpg">
          </el-carousel-item>
          <el-carousel-item>
            <img src="../assets/6.jpg">
          </el-carousel-item>
          <el-carousel-item>
            <img src="../assets/7.jpg">
          </el-carousel-item>
          <el-carousel-item>
            <img src="../assets/8.jpg">
          </el-carousel-item>
        </el-carousel>
      </el-col>
      <el-col :span="7">
        <el-carousel
          :interval="3000"
          height="200px"
        >
          <el-carousel-item>
            <img src="../assets/1.jpg">
          </el-carousel-item>
          <el-carousel-item>
            <img src="../assets/2.jpg">
          </el-carousel-item>
          <el-carousel-item>
            <img src="../assets/3.jpg">
          </el-carousel-item>
          <el-carousel-item>
            <img src="../assets/4.jpg">
          </el-carousel-item>
        </el-carousel>
      </el-col>
    </el-row>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
export default {
  name: "home",
  components: {
    HelloWorld
  }
};
</script>
<style lang="less" scoped>
.home {
  background: url(../assets/bg1.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  -webkit-background-size: cover;
  background-position: center 0;
  padding: 20px 0;
  .info{
    padding:0px 0 20px 200px;
    color: #909090;
    p{
      font-size: 26px;
    }
    h1{
      font-size: 50px;
    }
  }
  img {
    height: 250px;
    width: 100%;
  }
  .row-lb {
    padding: 0px 150px 20px;
    .el-carousel__item h3 {
      color: #475669;
      font-size: 14px;
      opacity: 0.75;
      line-height: 200px;
      margin: 0;
    }
    .el-carousel__item {
      border-radius: 10px;
    }
  }
}
</style>
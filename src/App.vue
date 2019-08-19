<template>
  <div id="app">
    <div class="heater">
      <div class="icon">
        <img src="./assets/logo.png">
        <span>上海昶满岳科技有限公司</span>
      </div>
      <div class="nav">
        <el-menu
          :default-active="$route.path"
          router
          mode="horizontal"
          @select="handleSelect"
          background-color="#000"
          text-color="#fff"
          active-text-color="#42b983"
        >
          <el-menu-item index="/">首页</el-menu-item>
          <!-- <el-submenu index="2">
            <template slot="title">关于我们</template>
            <el-menu-item index="2-1">公司简介</el-menu-item>
            <el-menu-item index="2-2">主要产品</el-menu-item>
            <el-menu-item index="2-3">应用场景</el-menu-item>
          </el-submenu> -->
          <el-menu-item index="/about">关于我们</el-menu-item>
          <el-menu-item index="/product">主要产品</el-menu-item>
          <el-menu-item index="/application">应用场景</el-menu-item>
          <el-menu-item index="/join">加入我们</el-menu-item>
          <el-menu-item index="/telephone">联系我们</el-menu-item>
        </el-menu>
        <!-- <router-link to="/">首页</router-link> |
        <router-link to="/about">关于我们</router-link> -->
      </div>
    </div>
    <div class="body">
      <router-view />
    </div>
    <div class="footer">
      <div class="telephone">
        <i class="el-icon-mobile"></i><span> 132-2106-1235 </span>
        <i class="el-icon-message"></i><span> shcmykj@gdy.cn </span>
        <i class="el-icon-chat-dot-square"></i><span> 微信 </span>
      </div>
      <div class="address">
        <i class="el-icon-map-location"></i><span>上海市金山区物联网街451号 芯图大厦</span>
      </div>
      <div>

      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      html: '<img src="./assets/wx.png">',
      acticeIndex: "/"
    };
  }
};
</script>
<style lang="less">
body {
  margin: 0;
  padding: 0;
}
#app {
  .nav {
    .el-menu-item:hover,
    .el-submenu:hover {
      background: #333 !important;
    }
  }
}
</style>
<style lang="less" scoped>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  color: #2c3e50;
  // height: 100%;
  .heater {
    position: fixed;
    top: 0;
    left: 0;
    z-index: 1000;
    width: 100%;
    height: 60px;
    background-color: #000;
    .icon {
      float: left;
      color: #fff;
      line-height: 60px;
      padding-left: 55px;
      img {
        position: absolute;
        top: 15px;
        left: 20px;
        width: 30px;
        height: 30px;
      }
    }
    .nav {
      float: right;
    }
  }
  .body {
    padding-top: 60px;
  }
  .footer {
    height: 100px;
    padding-top: 20px;
    // line-height: 100px;
    text-align: center;
    background: #000;
    color: #fff;
    div {
      padding: 10px 0px 0px 20px;
    }
    span {
      color: #686868;
      padding: 0 20px 0 5px;
      font-size: 14px;
    }
  }
}
// #nav {
//   padding: 30px;
//   a {
//     font-weight: bold;
//     color: #2c3e50;
//     &.router-link-exact-active {
//       color: #42b983;
//     }
//   }
// }
</style>

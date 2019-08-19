<template>
  <div class="application">
    <h1>应用场景</h1>
    <div>
      <el-row>
        <el-col
          :span="11"
          v-for="(o, index) in 2"
          :key="o"
          :offset="index > 0 ? 2 : 0"
          style="padding-bottom:30px"
        >
          <el-card > 
            <img src="../assets/jc.png">
            <div style="text-align:center;padding:10px">
              <span>好用的设备</span>
              <div class="bottom clearfix">
                <el-button
                  type="text"
                  class="button"
                >查看更多>></el-button>
              </div>
            </div>
          </el-card>
        </el-col>
      </el-row>
      <el-row>
        <el-col
          :span="11"
          v-for="(o, index) in 2"
          :key="o"
          :offset="index > 0 ? 2 : 0"
        >
          <el-card>
            <img src="../assets/jc.png">
            <div style="text-align:center;padding:10px">
              <span>好用的设备</span>
              <div class="bottom clearfix">
                <el-button
                  type="text"
                  class="button"
                >查看更多>></el-button>
              </div>
            </div>
          </el-card>
        </el-col>
      </el-row>
      
    </div>
  </div>
</template>
<style lang="less" scoped>
.application {
  padding: 20px 200px;
  .time {
    font-size: 13px;
    color: #999;
  }
  .bottom {
    margin-top: 13px;
    line-height: 12px;
  }
  .button {
    padding: 0;
    float: right;
    color: #08e;
  }
  .image {
    width: 100%;
    display: block;
  }

  .clearfix:before,
  .clearfix:after {
    display: table;
    content: "";
  }

  .clearfix:after {
    clear: both;
  }
}
</style>
<template>
  <div id="cmodule">
    <!-- 导航栏 -->
    <el-container>
      <NavMemu/>
      <!-- 主体头部 -->
      <el-container>
        <el-header>
          <div class="header-title">Echarts图表展示</div>
        </el-header>
        <!-- 主体内容 -->
        <el-main class="conBox">
          <router-view/>
        </el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script setup>
import NavMemu from './views/NavMemu.vue';


</script>

<style>
.header-title {
  color: purple;
  font-size: 20px;
  font-weight: bold;
  text-align: center;
  height: 70px;
  line-height: 70px;
  /* border: solid 1px rgb(255, 0, 0); */
}

.chartCss {
  height: 600px;
  width: 80%;
  text-indent: 2em;
}

.conBox{
  background: rgba(16, 27, 49, .6);
}
</style>
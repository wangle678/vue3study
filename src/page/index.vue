<template>
  <div>
      <div class="side-navbar">
          <div class="navbar-title" v-for="item in sideNavbarData" :key="item.id">{{item.bigTitle}}</div>
      </div>
  </div>
</template>

<script>
export default {
    name: "index",
    data() {
        return {
            sideNavbarData: [
                {
                    id: 1,
                    bigTitle: "基础"
                },
                {
                    id: 2,
                    bigTitle: "深入组件"
                },
                {
                    id: 3,
                    bigTitle: "过渡 & 动画"
                },
                {
                    id: 4,
                    bigTitle: "可复用 & 组合"
                },
                {
                    id: 5,
                    bigTitle: "高阶指南"
                },
                {
                    id: 6,
                    bigTitle: "工具"
                },
                {
                    id: 7,
                    bigTitle: "规模化"
                },
                {
                    id: 8,
                    bigTitle: "无障碍"
                },
            ]
        }
    }
}
</script>

<style>
body {
    margin: 0px;
    padding: 0px;
}
.side-navbar {
    width: 200px;
    height: 100vh;
    overflow: auto;
    padding-left: 10px;
    background-color: pink;
}
.side-navbar .navbar-title {
    font-size: 20px;
}
</style>
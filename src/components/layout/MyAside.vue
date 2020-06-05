<template>
  <div class="aside">
    <div class="title">
      <p>HC小区管理系统</p>
    </div>
    <div v-for="(item,idx) in navs" :key="idx">
      <router-link tag="span" :to="item.path" active-class="nav_on" exact>
        <div class="nav">
          <i class="fa" :class="item.icon"></i>
          <span v-text="item.text"></span>
        </div>
      </router-link>
    </div>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      navs: [
        { path: "", text: "小区管理", icon: "fa-tag", id: 1 },
        { path: "/shop", text: "资产管理", icon: "fa-calendar", id: 2 },
        { path: "/good", text: "业主管理", icon: "fa-tag", id: 3 },
        { path: "/order", text: "费用管理", icon: " fa-hand-o-left", id: 4 },
        { path: "/customer", text: "智慧服务", icon: "fa-home", id: 5 },
        { path: "", text: "智慧停车", icon: "fa-tag", id: 6 },
        { path: "/shop", text: "保修管理", icon: "fa-calendar", id: 7 },
        { path: "/good", text: "组织管理", icon: "fa-tag", id: 8 },
        { path: "/order", text: "采购管理", icon: " fa-hand-o-left", id: 9 },
        { path: "/customer", text: "设备管理", icon: "fa-home", id: 10 },
        { path: "", text: "系统管理", icon: "fa-tag", id: 11 },
        { path: "/shop", text: "巡检管理", icon: "fa-calendar", id: 12 }
      ]
    };
  }
};
</script>

<style lang='scss'>
.aside {
  height: 100%;
  width: 100%;
  background: rgba(68, 68, 68, 1);
  .nav {
    color: #aaa;
    line-height: 50px;
    text-align: center;
    font-size: 14px;
    cursor: pointer;
    > span {
      padding-left: 5px;
    }
  }

  .nav:hover {
    background: rgba(102, 102, 102, 1);
    color: white;
  }
  .nav_on .nav {
    background: white;
    color: black;
  }
  .title {
    height: 80px;
    box-sizing: border-box;
    padding-top: 20px;
    text-align: center;
    > i {
      display: inline-block;
      width: 40px;
      height: 40px;
      line-height: 40px;
      border-radius: 50%;
      background: white;
      font-size: 24px;
      color: rgba(238, 0, 0, 1);
      cursor: pointer;
    }
  }
}
</style>

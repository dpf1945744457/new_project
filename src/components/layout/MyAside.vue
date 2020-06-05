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
        { path: "/order", text: "订单", icon: " fa-hand-o-left", id: 4 },
        { path: "/customer", text: "客户", icon: "fa-home", id: 5 },
        { path: "/ss", text: "数据", icon: "fa-book", id: 6 },
        { path: "/ss", text: "资产", icon: " fa-hand-o-left", id: 7 },
        { path: "/ss", text: "应用", icon: " fa-hand-o-left", id: 8 },
        { path: "/ss", text: "设置", icon: " fa-hand-o-left", id: 9 }
      ]
    }
  }
}
</script>

<style>

</style>

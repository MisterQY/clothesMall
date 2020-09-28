<template>
  <tab-bar>
    <tab-bar-item curPath="/home" activeColor="#dd2277">
      <img slot="item-icon" src="@/assets/img/tabbar/home.png" alt="">
      <img slot="item-icon-active" src="@/assets/img/tabbar/home-active.png" alt="">
      <div slot="item-text">首页</div>
    </tab-bar-item>
    <tab-bar-item curPath="/category" activeColor="#dd2277">
      <img slot="item-icon" src="@/assets/img/tabbar/category.png" alt="">
      <img slot="item-icon-active" src="@/assets/img/tabbar/category-active.png" alt="">
      <div slot="item-text">分类</div>
    </tab-bar-item>
    <tab-bar-item curPath="/cart" activeColor="#dd2277">
      <img slot="item-icon" src="@/assets/img/tabbar/cart.png" alt="">
      <img slot="item-icon-active" src="@/assets/img/tabbar/cart-active.png" alt="">
      <div slot="item-text">购物车</div>
    </tab-bar-item>
    <tab-bar-item curPath="/profile" activeColor="#dd2277">
      <img slot="item-icon" src="@/assets/img/tabbar/profile.png" alt="">
      <img slot="item-icon-active" src="@/assets/img/tabbar/profile-active.png" alt="">
      <div slot="item-text">我的</div>
    </tab-bar-item>
  </tab-bar>
</template>

<script>
import TabBar from "@/components/tabbar/TabBar.vue"
import TabBarItem from "@/components/tabbar/TabBarItem.vue"

export default {
  name: "MainTabBar",
  components: {
    TabBar,
    TabBarItem,
  },
  data: () => ({

  })
}
</script>
<style scoped>
</style>

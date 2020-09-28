<template>
  <div class="navBarBlock">
    <!-- <slot></slot> -->
    <div class="navBar">
      <div class="NavBarItem">
        <img src="@/assets/img/navbar/left-arrow.png" alt="">
      </div>
      <div class="NavBarItem NavBarItemTitle">
        <div class="TitleContent">
          {{title}}
        </div>
      </div>
      <div class="NavBarItem">
        <img src="@/assets/img/navbar/menu.png" alt="">
      </div>

    </div>
  </div>
</template>

<script>
export default {
  name: "NavBar",
  computed: {
    title() {
      if( this.$route.path.indexOf('/home') != -1 ) {
        return '首页'
      }
      if( this.$route.path.indexOf('/category') != -1 ) {
        return '分类'
      }
      if( this.$route.path.indexOf('/cart') != -1 ) {
        return '购物车'
      }
      if( this.$route.path.indexOf('/profile') != -1 ) {
        return '我的'
      }
    }
  },
  data: () => ({

  })
}
</script>

<style scoped>

.navBarBlock {
  position: fixed;
  right: 0;
  left: 0;
  top: 0;
  height: 44px;
  background-color: #dd2277;
  display: flex;
}

.navBar {
  position: fixed;
  right: 0;
  left: 0;
  top: 0;
  height: 44px;
  background-color: #dd2277;
  display: flex;
}

.NavBarItem {
  flex: 60;
  text-align: center;
}

.NavBarItem img {
  margin-top: 10px;
  width: 24px;
  height: 24px;
}

.TitleContent {
  color: #ffffff;
  font-size: 16px;
  text-align: center;
  line-height: 44px;

}

.NavBarItemTitle {
  flex: 315;
}
</style>

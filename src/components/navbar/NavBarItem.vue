<template>
  <div class="NavBarItem">
    <div class="NavBarItem backButton"><slot name="back-button"></slot></div>
    <div class="NavBarItem pageTitle"><slot name="page-title"></slot></div>
    <div class="NavBarItem selectMenu"><slot name="select-menu"></slot></div>
  </div>
</template>

<script>
export default {
  name: "NavBarItem",
  data: () => ({

  })
}
</script>

<style scoped>
.NavBarItem {
  /* flex: 1; */
}

.backButton {
}

.backButton img {
  margin-top: 8px;
  width: 28px;
  height: 28px;
}

.pageTitle {
  color: #ffffff;
  font-size: 14px;
  text-align: center;
  line-height: 44px;
  width: 200px;
  border: 1px solid #000000;
}

.selectMenu img {
  margin-top: 8px;
  width: 28px;
  height: 28px;
}
</style>

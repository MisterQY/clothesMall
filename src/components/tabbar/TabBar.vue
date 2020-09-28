<template>
  <div class="tabbarBlock">
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: "TabBar"
}
</script>

<style lang="css" scoped>

.tabbarBlock {
  position: fixed;
  right: 0;
  left: 0;
  bottom: 0;
  background-color: #e8e8e8;
  height: 49px;
  display: flex;
  font-size: 12px;
}

</style>

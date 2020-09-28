<template lang="html">
  <div class="tabbarItem" @click="itemClick">
    <div v-if="!isActive"><slot name="item-icon"></slot></div>
    <div v-if="isActive"><slot name="item-icon-active"></slot></div>
    <div style="color: #707070" v-if="!isActive">
      <slot name="item-text"></slot>
    </div>
    <div :style="'color:' + activeColor " v-if="isActive">
      <slot name="item-text"></slot>
    </div>
  </div>
  </div>
</template>

<script>
export default {
  name: "TabBarItem",
  props: {
    curPath: String,
    activeColor: String
  },
  data() {
    return {
      originColor: '#707070'
    }
  },
  computed: {
    isActive() {
      return this.$route.path.indexOf(this.curPath) != -1
    }
  },
  methods: {
    itemClick() {
      this.$router.replace(this.curPath)
    }
  }
}
</script>

<style lang="css" scoped>

.tabbarItem {
  flex: 1;
  text-align: center;
  margin-top: 6px;
}

.tabbarItem img {
  height: 20px;
  width: 20px;
}

</style>

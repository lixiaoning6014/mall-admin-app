<template>
  <div class="home">
    <LeftMenu />
    <!-- 只有左边菜单缩进去了就让他触发 menu-unfold-->
    <div :class="{'main-app':true,'menu-unfold' : collapsed}">
      <SliderNav />
    </div>
  </div>
</template>

<script>
  import LeftMenu from '@/component/menu.vue';
  import SliderNav from '@/component/sliderNav.vue';
  export default {
    data() {
      return {
        collapsed: false,
      };
    },
    components: {
      LeftMenu,
      SliderNav
    },
    methods: {
      toggleCollapsed() {
        this.collapsed = !this.collapsed;
      }
    }
  }
</script>
<style lang="less">
  // 加上一个~让他当成模块来进行编译
  @import url("~@/assets/css/home.less");
</style>
<template>
  <div id="app">
    <BaseHeader/>
    <BaseMain/>
    <BaseFooterTop/>
    <BaseFooterMiddle/>
    <BaseFooterBottom/>
  </div>
</template>

<script>
import BaseHeader from "./components/blocks/BaseHeader.vue";
import BaseMain from "./components/blocks/BaseMain.vue";
import BaseFooterTop from "./components/blocks/footer/BaseFooterTop.vue";
import BaseFooterMiddle from "./components/blocks/footer/BaseFooterMiddle.vue";
import BaseFooterBottom from "./components/blocks/footer/BaseFooterBottom.vue";

export default {
  name: 'App',
  components: {
    BaseHeader,
    BaseMain,
    BaseFooterTop,
    BaseFooterMiddle,
    BaseFooterBottom
}
}
</script>

<style lang="scss">
@import "./assets/style/global.scss";
</style>

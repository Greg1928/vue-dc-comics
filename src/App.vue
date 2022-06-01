<template>
  <div id="app">
    <BaseHeader/>
    <BaseMain/>
    <BaseFooterTop/>
    <BaseFooterMiddle/>
  </div>
</template>

<script>
import BaseHeader from "./components/BaseHeader.vue";
import BaseMain from "./components/BaseMain.vue";
import BaseFooterTop from "./components/footer/BaseFooterTop.vue";
import BaseFooterMiddle from "./components/footer/BaseFooterMiddle.vue";

export default {
  name: 'App',
  components: {
    BaseHeader,
    BaseMain,
    BaseFooterTop,
    BaseFooterMiddle
}
}
</script>

<style lang="scss">
@import "./assets/style/global.scss";
</style>

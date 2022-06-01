<template>
  <div id="app">
    <BaseHeader/>
    <BaseMain/>
    <BaseFooterTop/>
  </div>
</template>

<script>
import BaseHeader from "./components/BaseHeader.vue";
import BaseMain from "./components/BaseMain.vue";
import BaseFooterTop from "./components/footer/BaseFooterTop.vue";

export default {
  name: 'App',
  components: {
    BaseHeader,
    BaseMain,
    BaseFooterTop,
}
}
</script>

<style lang="scss">
@import "./assets/style/global.scss";
</style>

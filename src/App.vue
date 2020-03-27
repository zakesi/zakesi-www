<template>
  <div id="app" class="page-layout">
    <BasicHeader />
    <div class="page-body">
      <router-view />
    </div>
    <BasicFooter />
  </div>
</template>

<script type="text/javascript">
import BasicHeader from "@/components/BasicHeader.vue";
import BasicFooter from "@/components/BasicFooter.vue";

export default {
  components: {
    BasicHeader,
    BasicFooter
  }
};
</script>

<style lang="less">
html,
body,
#app {
  height: 100%;
}
body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
    "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji",
    "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";
  color: #333;
  min-width: 1080px;
  margin: 0;
}
.container-1240 {
  max-width: 1240px;
  margin: 0 auto;
  padding: 0 20px;
}
.page-body {
  min-height: calc(100vh - 72px - 284px);
}
a {
  text-decoration: none;
}
</style>

<template>
  <header class="page-header">
    <div class="header-content">
      <div class="header-hd">
        <img
          v-if="false"
          class="header-logo"
          src="@/assets/images/logo/logo-white.png"
        />
        <h1 class="header-title">扎克斯 - 沉浸式编程学习</h1>
      </div>
      <div class="header-bd"></div>
      <div class="header-ft">
        <nav class="header-nav">
          <router-link class="header-nav-item" :to="{ name: 'Home' }"
            >编程学习</router-link
          >
          <router-link class="header-nav-item" :to="{ name: 'About' }"
            >关于我们</router-link
          >
        </nav>
      </div>
    </div>
  </header>
</template>
<script type="text/javascript">
export default {
  data() {
    return {};
  },
  computed: {},
  methods: {}
};
</script>
<style type="text/css" lang="less" scoped>
.page-header {
  height: 72px;
  background-color: #252222;
  // background-color: #fff;
  box-shadow: 0px 0px 10px 0px rgba(0, 0, 0, 0.05);
  z-index: 1;
  font-weight: 400;
  color: #fff;
  .header-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-left: 20px;
    .header-hd,
    .header-bd,
    .header-ft {
      display: flex;
      align-items: center;
      height: 72px;
      .el-icon-search {
        cursor: pointer;
      }
    }

    .header-logo {
      height: 28px;
      margin-right: 15px;
      vertical-align: middle;
    }

    .header-title {
      margin-right: 60px;
      font-size: 22px;
      font-weight: 400;
    }

    .header-nav {
      display: flex;
      align-items: center;
      height: 72px;
      .header-nav-item {
        position: relative;
        display: flex;
        align-items: center;
        font-size: 14px;
        height: 20px;
        line-height: 20px;
        margin-right: 35px;
        text-decoration: none;
        cursor: pointer;
        color: #fff;
        &.router-link-exact-active {
          &:after {
            position: absolute;
            content: "";
            width: 110%;
            height: 3px;
            background: rgba(15, 199, 0, 1);
            bottom: -6px;
            left: 50%;
            transform: translateX(-50%);
          }
        }
      }
    }

    .page-header-right {
      height: 100%;
    }

    .bar-info-container {
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100%;
      padding: 0 15px;
      transition: all 0.2s ease;
      cursor: pointer;
      &:hover {
        background-color: rgb(235, 248, 238);
      }
      &.logout {
        width: 105px;
        height: 32px;
        background-color: #1e1e1e;
        color: rgba(255, 255, 255, 1);
        font-size: 12px;
        cursor: pointer;
        &:hover {
          opacity: 0.8;
        }
      }
      .userInfo-name {
        height: 17px;
        line-height: 17px;
        font-weight: 400;
        font-size: 12px;
        color: #1e1e1e;
        vertical-align: middle;
      }
      .userInfo-avatar-container {
        position: relative;
        .userInfo-avatar {
          display: inline-block;
          width: 32px;
          height: 32px;
          background-color: #f1f1f1;
          border-radius: 50%;
          outline: none;
          margin-right: 12px;
        }
        .userInfo-vip {
          display: inline-block;
          height: 24px;
          width: 24px;
          position: absolute;
          bottom: 0;
          right: 0;
        }
      }
    }
  }
}
</style>

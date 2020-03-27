<template>
  <div>
    <div class="footer-section">
      <div class="container-1240">
        <div class="footer-vertical_top">
          <div class="logo-container" v-if="false">
            <router-link to="/">
              <img
                class="footer-logo"
                src="@/assets/images/logo/logo-white.png"
              />
            </router-link>
            <div class="logo-desc">
              面向未来的技术人才教育
            </div>
          </div>
          <div class="phone-container">
            <div class="phone-title">
              客服电话
            </div>
            <div class="phone-number">
              13502222677
            </div>
            <a href="/about" class="phone-contact" target="_blank">
              联系我们 👆
            </a>
          </div>
          <nav class="nav-container">
            <div class="nav-list">
              <div class="item-title">
                关于
              </div>
              <a href="/about" target="_blank" class="nav-item">关于我们</a>
            </div>
            <div class="nav-list" v-if="false">
              <div class="item-title">
                合作
              </div>
              <a
                href="https://shimo.im/forms/eVMAPV29oJgFmqg8/fill?channel=jiker-web"
                target="_blank"
                class="nav-item"
                >企业合作</a
              >
            </div>
            <div class="nav-list" v-if="false">
              <div class="item-title">
                支持
              </div>
              <a
                href="https://shimo.im/forms/15rk9dzJNRMTdqxP/fill?channel=jiker-web"
                target="_blank"
                class="nav-item"
                >意见反馈</a
              >
            </div>
          </nav>
        </div>
        <div class="footer-vertical_bottom">
          <div class="copyright-container">
            Copyright © 2018 扎克斯体验技术部出品
            <a href="http://www.beian.miit.gov.cn" target="_blank"
              >粤ICP备18089899号</a
            >
            粤公网安备 44011802000279号
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script type="text/javascript" scoped>
export default {
  data() {
    return {};
  }
};
</script>

<style type="text/css" lang="less" scoped>
.footer-section {
  background-color: #252222;
  font-weight: 400;
  padding: 45px 0 57px;
}
.footer-vertical_top {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  padding-bottom: 34px;
  border-bottom: 1px solid #414141;
  .logo-container {
    .footer-logo {
      height: 34px;
      margin-bottom: 15px;
    }
    .logo-desc {
      height: 17px;
      line-height: 17px;
      font-size: 14px;
      color: rgba(187, 187, 187, 1);
      letter-spacing: 2px;
      margin: 0;
    }
  }
  .phone-container {
    text-align: left;
    .phone-title {
      height: 22px;
      margin-bottom: 6px;
      line-height: 22px;
      font-size: 16px;
      font-weight: 600;
      color: rgba(255, 255, 255, 1);
    }
    .phone-number {
      height: 28px;
      line-height: 28px;
      font-size: 20px;
      color: rgba(213, 213, 213, 1);
      margin-bottom: 11px;
    }
    .phone-contact {
      display: inline-block;
      width: 255px;
      height: 43px;
      background-color: rgba(51, 51, 51, 1);
      text-align: center;
      font-size: 12px;
      line-height: 43px;
      color: rgba(255, 255, 255, 1);
      transition: 0.2s ease;
      &:hover {
        opacity: 0.8;
      }
    }
  }
  .nav-container {
    display: flex;
    align-items: flex-start;
    justify-content: space-between;
    padding-right: 28px;
    .nav-list {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      margin-right: 50px;
      .item-title {
        height: 22px;
        line-height: 22px;
        font-size: 16px;
        font-weight: 600;
        color: rgba(255, 255, 255, 1);
        margin-bottom: 12px;
      }
      .nav-item {
        height: 20px;
        line-height: 20px;
        color: #d5d5d5;
        font-size: 14px;
        margin-bottom: 14px;
        font-weight: 400;
        &:last-child {
          margin-bottom: 0;
        }
        &:hover {
          color: #fff;
        }
      }
      a {
        display: inline-block;
      }
      &:last-child {
        margin-right: 0;
      }
    }
  }
}
.footer-vertical_bottom {
  padding: 20px 0 0;
  .copyright-container {
    height: 17px;
    line-height: 17px;
    font-size: 12px;
    font-weight: 300;
    line-height: 17px;
    color: rgba(142, 142, 142, 1);
    text-align: right;
    > a {
      color: #fff;
    }
  }
}
</style>

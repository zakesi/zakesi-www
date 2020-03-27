<template>
  <div class="home-page">
    <div class="banner-section">
      <div class="container-1240">
        <div class="banner-content">
          <div class="banner-feature">
            <div class="banner-feature-item">零 - 讲授 / ZERO TUITION</div>
            <div class="banner-feature-item">零 - 老师 / ZERO TEACHERS</div>
            <div class="banner-feature-item">零 - 班级 / ZERO CLASSES</div>
          </div>
          <div class="banner-description">
            起源《最终幻想 IV · 核心危机
            》，一个以游戏通关模式打造的沉浸式编程学习空间。<br />
            1 ：1 还原企业工作场景，任务化的学习模式，每天组队打怪升级，从 1 ～
            21 级满级毕业。
          </div>
        </div>
      </div>
    </div>
    <div class="intro-section">
      <Partner
        class="container-1240"
        content="从零开始挑战实战项目，成为网站开发、移动开发和数据分析领域的抢手人才"
      />
    </div>
    <div class="market-section">
      <Market class="container-1240" />
    </div>
    <div class="feature-section">
      <Feature class="container-1240" />
    </div>

    <Advangate />
    <Try />
  </div>
</template>

<script type="text/javascript">
import Partner from "@/components/lp/Partner";
import Feature from "@/components/lp/Feature";
import Market from "@/components/lp/Market";
import Advangate from "@/components/lp/Advangate";
import Try from "@/components/lp/Try";

export default {
  data() {
    return {};
  },
  components: {
    Market,
    Partner,
    Feature,
    Advangate,
    Try
  }
};
</script>

<style type="text/css" lang="less">
.banner-section {
  position: relative;
  height: 50vh;
  min-height: 300px;
  background-image: url(https://assets.jiker.com/_for_plus_sub_project/2020/0306/admin/feeodrYoukYOYG58PNzpeaaaP31KOtso2N48jaBU.jpeg);
  background-position: center;
  background-size: cover;
  &:before {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.7);
    content: "";
  }
  .banner-content {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    color: #fff;

    .banner-feature-item {
      font-size: 40px;
      line-height: 1.6;
    }

    .banner-description {
      font-size: 16px;
      line-height: 2;
      margin-top: 16px;
    }
  }
}
</style>

<template>
  <div class="try-section">
    <div class="container-1240">
      <div class="try-title">名额有限！抢完即止</div>
      <div class="progress-list">
        <div class="progress-item">1. 预定超值 7 天试学</div>
        <div class="progress-item">2. 试学通过优先获得正式课程席位</div>
        <div class="progress-item">3. 毕业获得认证，实现理想改变未来</div>
      </div>
      <div class="try-content">
        <div class="card-insert">
          <h6 class="card-tips">开放预定中！</h6>
          <p class="card-title">扎克斯前端编程 30 天试学营</p>
          <div class="card-price-container">
            <span class="card-total-price">¥18800</span>
            <span class="card-try-price">¥880</span>
          </div>
          <ul class="card-desc-list">
            <li>提前体验企业工作场景</li>
            <li>掌握企业协同流程以及工具</li>
            <li>完成第一个 Web 实战作品</li>
            <li>拥有 UI 设计稿还原能力</li>
          </ul>
          <a href="javascript:;" class="card-btn" v-if="false">试听课程</a>
        </div>
        <div class="question-list">
          <div class="question-item">
            <p class="question-title">为什么需要试学？不能直接加入吗？</p>
            <p class="question-desc">
              高强度的编程未必适合任何人，自驱式的学习方式也未必适合所有人。<br />
              我们提供 30 天足够长的时间来适应。希望你真心想学，并能享受其中。
            </p>
          </div>
          <div class="question-item">
            <p class="question-title">为什么席位有限，需要预定？</p>
            <p class="question-desc">
              这里并不是养猪场，导师也不能服务一万人。<br />
              每年只有 40 个席位，我们能保证输出的 40 名都是都是行业的正规军。
            </p>
          </div>
          <div class="question-item">
            <p class="question-title">试学班学费是否可以抵扣正式费用？</p>
            <p class="question-desc">
              在你通过试学项目后，试学学费可以抵扣后续加入正式学费。<br />
              你还有机会获得额外的“项目奖学金”！
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "plan_try",
  data() {
    return {};
  }
};
</script>
<style scoped lang="less">
.try-section {
  padding: 40px 0 120px;
  background: url("https://cn.udacity.com/assets/iridium/images/nanodegree-overview/shared/nd-overview/svip-bg.jpg")
    center center/contain no-repeat;

  .try-title {
    font-size: 32px;
    font-weight: 400;
    color: #333;
    margin-bottom: 64px;
    line-height: 36px;
    text-align: center;
  }

  .progress-list {
    background-color: #fff;
    box-shadow: 0 2px 2px 0 rgba(46, 60, 73, 0.05);
    border: 1px solid #dbe2e8;
    border-radius: 6px;
    font-size: 18px;
    font-weight: 600;
    color: #2e3d49;
    margin-bottom: 40px;
    display: flex;

    .progress-item {
      position: relative;
      flex: 1;
      line-height: 34px;
      padding: 16px;
      text-align: center;

      &:not(:first-child) {
        border-left: 1px solid #dbe2e8;

        &:after {
          position: absolute;
          top: 50%;
          right: 0;
          bottom: 0;
          left: -0.3em;
          background-color: #fff;
          width: 0.6em;
          height: 0.6em;
          -webkit-transform: translateY(-50%) rotate(-45deg);
          transform: translateY(-50%) rotate(-45deg);
          content: "";
          border-right: 1px solid #dbe2e8;
          border-bottom: 1px solid #dbe2e8;
        }
      }
    }
  }

  .try-content {
    display: flex;
    justify-content: center;

    .card-insert {
      position: relative;
      width: 300px;
      padding: 48px 36px;
      background: #fff;
      box-shadow: 5px 5px 25px 0 rgba(46, 61, 73, 0.2);
      border-radius: 0.375rem;
      transition: all 0.3s ease;

      .card-tips {
        position: absolute;
        left: 0px;
        top: -8px;
        line-height: 28px;
        padding: 0 12px;
        color: #333;
        background-color: rgba(0, 0, 0, 0.1);
        font-size: 13px;
        font-weight: 600;
        letter-spacing: 2px;
        line-height: 28px;

        &:after {
          position: absolute;
          content: "";
          top: 0;
          width: 0;
          height: 0;
          right: -1rem;
          border-style: solid;
          -webkit-transform: rotate(360deg);
          transform: rotate(360deg);
          border-width: 1.75rem 1rem 0 0;
          border-color: rgba(0, 0, 0, 0.1) transparent transparent;
        }
      }

      .card-title {
        font-size: 18px;
        font-weight: 600;
        line-height: 32px;
        font-weight: 600;
        text-align: center;
      }

      .card-price-container {
        height: 80px;
        font-weight: 400;
        display: flex;
        justify-content: center;
        align-items: baseline;
        border-bottom: 2px solid #333;
        margin-bottom: 24px;
        .card-total-price {
          color: #999;
          font-size: 27px;
          text-decoration-line: line-through;
          margin-right: 10px;
        }
        .card-try-price {
          color: #333;
          font-size: 39px;
        }
      }

      .card-desc-list {
        li {
          font-size: 16px;
          color: #666;
          font-size: 400;
          line-height: 32px;
        }
      }

      .card-btn {
        display: block;
        cursor: pointer;
        text-align: center;
        text-decoration: none;
        vertical-align: middle;
        height: 3rem;
        padding: 0 0.5rem;
        text-transform: uppercase;
        font-weight: 600;
        font-size: 16px;
        line-height: 48px;
        height: 48px;
        border-radius: 0.25rem;
        letter-spacing: 0.125rem;
        transition: all 0.3s ease;
        color: #fff;
        background-color: #02b3e4;
        border: 0.125rem solid transparent;
        box-shadow: 8px 10px 20px 0 rgba(46, 61, 73, 0.15);
        margin-top: 24px;
        &:hover {
          border-color: transparent;
          background-color: #029fcb;
          box-shadow: 2px 4px 8px 0 rgba(46, 61, 73, 0.2);
        }
      }
    }
    .question-list {
      padding-top: 20px;
      margin-left: 50px;
      width: 580px;
      font-weight: 400;

      .question-title {
        font-size: 24px;
        margin-bottom: 12px;
        line-height: 36px;
        color: #333;
      }

      .question-desc {
        font-size: 16px;
        color: #666;
        line-height: 28px;
        margin-bottom: 24px;
      }
    }
  }
}
</style>

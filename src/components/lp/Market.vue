<template>
  <div class="market-section">
    <div class="market-container">
      <div class="market-article-container">
        <h2 class="market-article-title">1 : 1 还原工作场景，沉浸式编程学习</h2>
        <div class="market-article-desc">
          <p>
            1 : 1
            还原真实的互联网工作环境，宽阔办公环境、舒适座椅、超快网络，以及一切项目开发你所需要的工具及专业书籍。专属的导师带入门，领取任务副本，每个任务都来自企业的真实需求。每天实战打怪升级，每个人都由自己的级别，从
            1 级到 21 级。
          </p>
          <p>
            在工作中遇到问题我们不能奢望总有人能够指导我们。身边的小伙伴，就是老师，专注培养团队协助以及独立解决问题的能力。毕业生（
            21 级）非常善于解决实际问题，很受公司的欢迎。
          </p>
          <p>相比于知识的灌溉，我们更关心你的能力的提升。</p>
        </div>
        <button class="market-aritcle-btn" v-if="false">试听课程</button>
      </div>
      <div class="market-card-container">
        <h2 class="market-card-tite">企业真实项目体系</h2>
        <div class="market-card-desc">
          <p>- 完全符合商用级上线应用标准</p>
          <p>- 产品需求及规划遵循用户需求</p>
          <p>- 具备一定体量功能及业务规模</p>
          <p>- 注重用户体验交互及视觉效果</p>
          <p>- 完全执行标准化研发管理流程</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "plan_market",
  data() {
    return {};
  }
};
</script>

<style scoped lang="less">
.market-container {
  display: flex;
  justify-content: space-between;

  .market-article-container {
    max-width: 780px;
    padding-right: 80px;

    .market-article-title {
      font-size: 32px;
      font-weight: 400;
      line-height: 36px;
      margin-bottom: 24px;
      color: #333;
    }

    .market-article-desc {
      font-size: 16px;
      font-weight: 400;
      line-height: 28px;
      color: #666;

      p {
        margin-bottom: 12px;
      }
    }

    .market-aritcle-btn {
      display: block;
      cursor: pointer;
      text-align: center;
      white-space: nowrap;
      text-decoration: none;
      vertical-align: middle;
      height: 3rem;
      padding: 0 0.5rem;
      text-transform: uppercase;
      font-weight: 600;
      font-size: 0.8125rem;
      line-height: 2.625rem;
      border-radius: 0.25rem;
      letter-spacing: 0.125rem;
      transition: all 0.3s ease;
      width: 13.75rem;
      color: #fff;
      background-color: #02b3e4;
      border: 0.125rem solid transparent;
      box-shadow: 8px 10px 20px 0 rgba(46, 61, 73, 0.15);
      margin-top: 40px;
      &:hover {
        border-color: transparent;
        background-color: #029fcb;
        box-shadow: 2px 4px 8px 0 rgba(46, 61, 73, 0.2);
      }
    }
  }

  .market-card-container {
    // width: 300px;
    flex-shrink: 0;
    text-align: left;
    position: relative;
    box-shadow: 5px 5px 25px 0 rgba(46, 61, 73, 0.2);
    border-radius: 0.375rem;
    transition: all 0.3s ease;
    background: #fff;
    box-shadow: 5px 5px 25px 0 rgba(46, 61, 73, 0.2);
    border-top: 3px solid #333;
    min-height: 15rem;
    padding: 2.25rem;

    .market-card-tite {
      font-size: 24px;
      font-weight: 400;
      line-height: 36px;
      margin-bottom: 12px;
      color: #333;
    }

    .market-card-desc {
      font-size: 14px;
      line-height: 1.5;
      letter-spacing: 1px;
      text-transform: uppercase;
      font-weight: 600;
      color: #999;
    }
  }
}
</style>

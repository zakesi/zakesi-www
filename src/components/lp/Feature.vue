<template>
  <div class="serve-section">
    <div class="serve-list">
      <div class="serve-item">
        <div
          class="serve-item-image"
          style="background-image: url(https://assets.jiker.com/_for_plus_sub_project/2020/0307/admin/PiiWI103Z3kBXeElfRV0fchW1cO6s93jelw2b6xu.jpg);"
        ></div>
        <div class="serve-detail-list">
          <div class="serve-detail-item">
            <img
              class="serve-detail-image"
              src="https://q2.cdn.prodegree.com/default/2020/0307/HQqpsCj6ld337xa9P6QbIalIdi2Y2vEM9UoxtVLO.svg"
            />
            <h3 class="serve-detail-title">没有讲授</h3>
            <p class="serve-detail-desc">
              和传统培训不同，没有 1 vs 40
              的传统讲授。通过系统化的学习体系以及精心挑选的学习资源，根据我们设定的游戏规则，一步一脚，踏实不虚。
            </p>
          </div>
          <div class="serve-detail-item">
            <img
              class="serve-detail-image"
              src="https://q2.cdn.prodegree.com/default/2020/0307/I5K80StMPvp6QY5jBpo3J9tlTECMnj7v31TiuAfr.svg"
            />
            <h3 class="serve-detail-title">没有老师</h3>
            <p class="serve-detail-desc">
              专属导师会领你一步一步熟悉规则，并对你的任务进行验收。你身边的伙伴就是你的老师，你也是其他伙伴的老师。
            </p>
          </div>
        </div>
      </div>
      <div class="serve-item">
        <div class="serve-detail-list">
          <div class="serve-detail-item">
            <img
              src="https://q2.cdn.prodegree.com/default/2020/0307/3fZ8P4UuVIb7Rdxtx5e91lpWMIwJqU4iEj8cWIdA.svg"
              class="serve-detail-image"
            />
            <h3 class="serve-detail-title">没有班级</h3>
            <p class="serve-detail-desc">
              每个人的学习能力、付出决定了学习进度，学习不可能做批量生产。是否毕业取决于是否有能力完成任务，和时间无关。我们保证输出结果，不保证时间。
            </p>
          </div>
          <div class="serve-detail-item">
            <img
              src="https://q2.cdn.prodegree.com/default/2020/0307/xEN7TWB9IDX0RbtcjzdgKdxCA8hLSS6lgA5Sa7Vj.svg"
              class="serve-detail-image"
            />
            <h3 class="serve-detail-title">只有编程</h3>
            <p class="serve-detail-desc">
              学习就是打怪升级，通过一个一个真实的任务，让你真正的得到能力的提升。从
              1 ～ 21 级，满级达到独立开发水平，能完成你能想象出来的作品。
            </p>
          </div>
        </div>
        <div
          class="serve-item-image"
          style="background-image: url(https://assets.jiker.com/_for_plus_sub_project/2020/0307/admin/Nbxy2BHAXXF9eYRrjLBTrj6HfFJm6ka5XxINA4BG.jpg)"
        ></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "plan_help",
  data() {
    return {};
  }
};
</script>
<style scoped lang="less">
.serve-section {
  .serve-list {
    padding: 40px 0;
  }
  .serve-item {
    display: flex;
    justify-content: space-between;
    margin-bottom: 60px;
    &:last-child {
      margin-bottom: 0;
    }
  }
  .serve-detail-list {
    display: inline-block;
    max-width: 680px;
    padding: 0 40px;

    .serve-detail-item {
      position: relative;
      padding-left: 80px;
    }
    .serve-detail-image {
      position: absolute;
      top: -10px;
      left: -10px;
      width: 80px;
      filter: grayscale(100%);
    }
    .serve-detail-title {
      font-size: 24px;
      line-height: 36px;
      color: #2e3d49;
      margin-bottom: 12px;
      font-weight: 400;
    }
    .serve-detail-desc {
      font-size: 16px;
      color: #525c65;
      line-height: 2;
      margin-bottom: 48px;
    }
  }
  .serve-item-image {
    position: relative;
    flex: 1;
    background-size: cover;
    transition: all 0.2s ease;
    opacity: 0.8;
    &:hover {
      opacity: 1;
      &:after {
        opacity: 0;
      }
    }
    &:after {
      transition: all 0.2s ease;
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(0, 0, 0, 0.4);
      content: "";
    }
  }
}
</style>

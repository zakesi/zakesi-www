<template>
  <div class="partner--section">
    <div class="partner--list">
      <div class="partner--item">
        <img
          class="partner--item__image"
          src="~@/assets/images/partners/logo-gray-google.svg"
        />
      </div>
      <div class="partner--item">
        <img
          class="partner--item__image"
          src="~@/assets/images/partners/logo-gray-facebook.svg"
        />
      </div>
      <div class="partner--item">
        <img
          class="partner--item__image"
          src="~@/assets/images/partners/logo-gray-amazon.svg"
        />
      </div>
      <div class="partner--item">
        <img
          class="partner--item__image"
          src="~@/assets/images/partners/logo-gray-ibm.svg"
        />
      </div>
      <div class="partner--item">
        <img
          class="partner--item__image"
          src="~@/assets/images/partners/logo-gray-github.svg"
        />
      </div>
      <div class="partner--item">
        <img
          class="partner--item__image"
          src="~@/assets/images/partners/logo-gray-tencent.svg"
        />
      </div>
      <div class="partner--item">
        <img
          class="partner--item__image"
          src="~@/assets/images/partners/logo-gray-didi.svg"
        />
      </div>
    </div>
    <div class="partner--description">{{ content }}</div>
  </div>
</template>

<script>
export default {
  name: "BaseMoreInfo",
  data() {
    return {};
  },
  props: {
    content: {
      type: String,
      default:
        "掌握 Google、Facebook、Tencent 等最前沿技术，成为行业抢手科技人才"
    }
  }
};
</script>

<style lang="less" scoped>
.partner--section {
  padding: 40px 0;
  .partner--list {
    opacity: 0.7;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
    border-bottom: 1px solid rgba(0, 0, 0, 0.1);
    .partner--item__image {
      max-height: 60px;
      margin: 0 24px;
      filter: grayscale(100%);
    }
  }
  .partner--description {
    color: #999;
    text-align: center;
    font-size: 16px;
    line-height: 60px;
  }
}
</style>

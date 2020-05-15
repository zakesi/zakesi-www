<template>
  <div class="about-page">
    <div class="video-section" v-if="false">
      <video
        ref="video"
        class="video-content"
        src="https://q2.cdn.prodegree.com/default/2020/0308/fMpfisVWHMKpoe11Xl3iFPdrnxci3c90xwGsDQD3.mp4"
      ></video>
      <div class="video-mask" @click="playVideo"></div>
    </div>
    <div class="article-section">
      <div class="article-content">
        <div class="article-title">编程，是一种信仰 !</div>
        <p>
          随着人工智能和机器学习的发展，无人汽车、机器人、大数据及自动化的普及
          ，未来 20年内，80%
          的现有工作行为可以被机器或者程序代替，甚至对现有知识进行整合重构。新的科技知识，大概每两年会增加一倍。对读大学的学生来说，很多他们在一年级、二年级所学的知识，在大三年级时就全部过时。技术的发展正快速更迭着人类维持生产力增长所需的能力，而现有教育体系已经无法满足这些需求。
        </p>

        <p>
          一件事情的起因蕴涵着它的基因，并指引着它的未来。2018年初，「 扎克斯编
          」正式启动，正是我们对这个时代的深度观察与思考。从招募到第一批初始学员，完成了一轮试课，及从培养目标、教学体系、IT系统等的整体搭建。通过一个优异的学习平台，整合高质量的资源，探索高效的学习方式，帮助学习者提高效率，拥有最好的知识和更远大的前程。我们希望在这个全新的时代中，对未来的教育进行探索，以新的内容，新的形式，为体制教育做一些新的补充，让学习更有价值。
        </p>

        <p>
          当古希腊第一次出现「 Schole
          」这个词的时候，它其实是闲暇的意思。它是一群人去思考，生命的意义是什么，幸福是什么，理想的国度是什么的场景。当工业革命时期时，教育开始变得更极度的实用主义，它彻底反映着社会的发展对于人的需求。在同样的场景里面、学习同样的知识、以同样的进度。然而就在人类即将步入当今这个时代，就在人工智能和机器即将代替大部分人类原有的时代。或许正式因为我们存在于这个时代，我们才有机会去回归教育最本质与美好的使命，去做真正以人类为中心，最能推动文明进展的教育。去重新定义，学校是什么？我们为什么而学？我们要学什么？
        </p>

        <p>
          教育不应只是年轻时一段暂时的经历，而是延续终生不断助人前行的动力；教育不应只是让学生被动接收灌输，而应引导他们主动参与，通过实战收获实用的技能；教育的目标不只是让学生在校园内获得成功，更要让他们一生受益并最终获得成功的人生。
        </p>

        <p>
          我们相信开源的力量，相信聚群的力量，我们憧憬着用最彻底的方式做出我们心中最理想教育模式。从心出发，未来快乐！
        </p>

        <div>
          <img
            class="article-img"
            src="https://vip-assets.jiker.com/for_neon_project/WechatIMG1.jpeg"
          />
          <img
            class="article-img"
            src="https://vip-assets.jiker.com/for_neon_project/WechatIMG2.jpeg"
          />
          <img
            class="article-img"
            src="https://vip-assets.jiker.com/for_neon_project/WechatIMG3.jpeg"
          />
          <img
            class="article-img"
            src="https://vip-assets.jiker.com/for_neon_project/WechatIMG6.jpeg"
          />
          <img
            class="article-img"
            src="https://vip-assets.jiker.com/for_neon_project/WechatIMG7.jpeg"
          />
          <img
            class="article-img"
            src="https://vip-assets.jiker.com/for_neon_project/WechatIMG8.jpeg"
          />
          <img
            class="article-img"
            src="https://vip-assets.jiker.com/for_neon_project/WechatIMG9.jpeg"
          />
          <img
            class="article-img"
            src="https://vip-assets.jiker.com/for_neon_project/WechatIMG10.jpeg"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script type="text/javascript">
export default {
  data() {
    return {};
  },
  computed: {},
  methods: {
    playVideo() {
      const video = this.$refs.video;
      video.play();
      video.webkitRequestFullScreen();
    }
  }
};
</script>

<style type="text/css" lang="less" scoped>
.video-section {
  height: 50vh;
  background-color: #333;
  position: relative;
  .video-content {
    height: 50vh;
    width: 100%;
    object-fit: cover;
    outline: none;
  }
  .video-mask {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    cursor: pointer;
    &:before {
      content: "";
      display: inline-block;
      width: 66px;
      height: 66px;
      position: absolute;
      top: 50%;
      left: 50%;
      margin-left: -33px;
      margin-top: -33px;
      background: #fff;
      border-radius: 50%;
      cursor: pointer;
    }
    &:after {
      content: "";
      display: inline-block;
      width: 0;
      height: 0;
      border-top: 14px solid transparent;
      border-bottom: 14px solid transparent;
      border-left: 22px solid #333;
      position: absolute;
      top: 50%;
      left: 50%;
      margin-top: -14px;
      margin-left: -6px;
    }
  }
}
.article-section {
  padding: 40px 0 120px;
  .article-title {
    font-size: 32px;
    margin-bottom: 32px;
    color: #333;
    text-align: center;
  }
}
.article-content {
  max-width: 700px;
  padding: 0 20px;
  margin: 0 auto;
  line-height: 2;
  font-size: 16px;
  p {
    text-indent: 30px;
  }
}

.article-img {
  max-width: 100%;
  margin: 10px auto;
}
</style>

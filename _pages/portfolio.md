---
layout: single
title: "作品集"
permalink: /portfolio/
author_profile: true
---
<style>
/* =========================================================
   PORTFOLIO
   ========================================================= */
.portfolio-page {
  width: 100%;
  max-width: 1500px;
  margin: 0 auto;
  padding: 20px 0 100px;
  color: #1f2724;
  font-family: -apple-system, BlinkMacSystemFont, "Helvetica Neue",
               "PingFang SC", "Microsoft YaHei", Arial, sans-serif;
}
.portfolio-page * {
  box-sizing: border-box;
}
.portfolio-page img {
  display: block;
  width: 100%;
  height: auto;
}
/* =========================================================
   COMMON
   ========================================================= */
.portfolio-section {
  margin-bottom: 150px;
}
.portfolio-section-label {
  display: flex;
  align-items: center;
  gap: 18px;
  margin-bottom: 45px;
  font-size: 12px;
  letter-spacing: 0.18em;
  text-transform: uppercase;
  color: #66726d;
}
.portfolio-section-label::after {
  content: "";
  width: 70px;
  height: 1px;
  background: #9da9a3;
}
.portfolio-section-title {
  margin: 0 0 15px;
  font-size: clamp(34px, 5vw, 72px);
  line-height: 0.95;
  font-weight: 500;
  letter-spacing: -0.04em;
}
.portfolio-section-description {
  max-width: 680px;
  margin: 0 0 45px;
  font-size: 14px;
  line-height: 1.9;
  color: #69736f;
}
/* =========================================================
   01 COVER
   ========================================================= */
.portfolio-cover {
  min-height: 78vh;
  display: grid;
  grid-template-columns: 0.9fr 1.4fr;
  gap: 55px;
  align-items: center;
  padding: 50px 0 100px;
}
.portfolio-cover-text {
  padding-right: 20px;
}
.portfolio-cover-number {
  margin-bottom: 30px;
  font-size: 12px;
  letter-spacing: 0.25em;
  color: #69746f;
}
.portfolio-cover-title {
  margin: 0;
  font-size: clamp(70px, 10vw, 150px);
  line-height: 0.82;
  letter-spacing: -0.07em;
  font-weight: 500;
}
.portfolio-cover-name {
  margin-top: 40px;
  font-size: 20px;
  letter-spacing: 0.08em;
}
.portfolio-cover-role {
  margin-top: 12px;
  font-size: 13px;
  color: #69746f;
  letter-spacing: 0.08em;
}
.portfolio-cover-meta {
  margin-top: 65px;
  padding-top: 20px;
  border-top: 1px solid rgba(31,39,36,0.25);
  font-size: 11px;
  line-height: 1.9;
  color: #737d79;
}
.portfolio-cover-image {
  position: relative;
  overflow: hidden;
  aspect-ratio: 4 / 5;
  background: #dfe4df;
}
.portfolio-cover-image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
/* =========================================================
   02 COPY & CAMPAIGN
   ========================================================= */
.copy-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 25px;
}
.copy-card {
  position: relative;
  min-height: 430px;
  padding: 45px;
  background: rgba(255,255,255,0.45);
  border: 1px solid rgba(31,39,36,0.12);
  transition: transform 0.35s ease,
              background 0.35s ease;
}
.copy-card:hover {
  transform: translateY(-8px);
  background: rgba(255,255,255,0.7);
}
.copy-card-number {
  font-size: 11px;
  letter-spacing: 0.18em;
  color: #78837e;
}
.copy-card-title {
  margin: 70px 0 30px;
  font-size: 34px;
  font-weight: 500;
}
.copy-card-copy {
  font-size: 18px;
  line-height: 1.9;
  letter-spacing: 0.03em;
}
.copy-card-info {
  position: absolute;
  left: 45px;
  bottom: 35px;
  font-size: 11px;
  line-height: 1.7;
  color: #737d79;
}
/* =========================================================
   CAMPAIGN
   ========================================================= */
.campaign-wrapper {
  margin-top: 100px;
}
.campaign-title {
  margin-bottom: 35px;
  font-size: 12px;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  color: #69746f;
}
.campaign-grid {
  display: grid;
  grid-template-columns: 1.3fr 0.7fr;
  gap: 30px;
  align-items: start;
}
.campaign-card {
  position: relative;
  overflow: hidden;
  background: #dfe4df;
}
.campaign-card img {
  aspect-ratio: 4 / 3;
  object-fit: cover;
  transition: transform 0.6s ease;
}
.campaign-card:hover img {
  transform: scale(1.04);
}
.campaign-card-info {
  padding: 24px 5px 10px;
}
.campaign-card-number {
  font-size: 10px;
  letter-spacing: 0.15em;
  color: #7a8580;
}
.campaign-card-name {
  margin-top: 8px;
  font-size: 25px;
}
.campaign-card-description {
  margin-top: 8px;
  font-size: 12px;
  line-height: 1.8;
  color: #707a76;
}
/* =========================================================
   SOCIAL
   ========================================================= */
.social-wrapper {
  margin-top: 100px;
}
.social-title {
  margin-bottom: 35px;
  font-size: 12px;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  color: #69746f;
}
.social-layout {
  position: relative;
  min-height: 700px;
}
.social-main {
  width: 72%;
}
.social-main img {
  aspect-ratio: 3 / 4;
  object-fit: cover;
}
.social-secondary {
  position: absolute;
  width: 37%;
  right: 0;
  bottom: 0;
  padding: 14px;
  background: #f5f6f2;
}
.social-secondary img {
  aspect-ratio: 3 / 4;
  object-fit: cover;
}
.social-caption {
  margin-top: 15px;
  font-size: 11px;
  line-height: 1.8;
  color: #707a76;
}
/* =========================================================
   03 VIDEO
   ========================================================= */
.video-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 25px;
}
.video-card {
  position: relative;
}
.video-media {
  position: relative;
  overflow: hidden;
  aspect-ratio: 16 / 9;
  background: #dce2dd;
}
.video-media img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.video-card-info {
  padding: 20px 3px;
}
.video-card-number {
  font-size: 10px;
  letter-spacing: 0.18em;
  color: #77817c;
}
.video-card-title {
  margin-top: 8px;
  font-size: 23px;
}
.video-card-description {
  margin-top: 8px;
  font-size: 12px;
  line-height: 1.8;
  color: #707a76;
}
/* =========================================================
   04 FEATURED CASE
   ========================================================= */
.featured-case {
  margin-top: 80px;
}
.case-header {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 50px;
  margin-bottom: 60px;
}
.case-header-title {
  font-size: clamp(45px, 7vw, 90px);
  line-height: 0.9;
  letter-spacing: -0.05em;
}
.case-header-description {
  align-self: end;
  font-size: 14px;
  line-height: 2;
  color: #69746f;
}
.case-cover {
  position: relative;
  overflow: hidden;
  aspect-ratio: 16 / 7;
  background: #dce2dd;
}
.case-cover img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.case-cover-label {
  position: absolute;
  left: 25px;
  bottom: 25px;
  padding: 8px 14px;
  background: rgba(255,255,255,0.85);
  font-size: 10px;
  letter-spacing: 0.12em;
}
/* PROCESS */
.case-process {
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  gap: 1px;
  margin-top: 70px;
  background: rgba(31,39,36,0.15);
}
.case-process-item {
  min-height: 190px;
  padding: 25px;
  background: rgba(255,255,255,0.35);
}
.case-process-number {
  font-size: 10px;
  color: #78827d;
  letter-spacing: 0.15em;
}
.case-process-title {
  margin-top: 35px;
  font-size: 18px;
}
.case-process-text {
  margin-top: 10px;
  font-size: 11px;
  line-height: 1.8;
  color: #737d79;
}
/* CASE IMAGES */
.case-images {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 25px;
  margin-top: 45px;
}
.case-image {
  overflow: hidden;
  background: #dce2dd;
}
.case-image img {
  aspect-ratio: 4 / 3;
  object-fit: cover;
  transition: transform 0.6s ease;
}
.case-image:hover img {
  transform: scale(1.03);
}
/* =========================================================
   05 VISUAL
   ========================================================= */
.visual-ae {
  margin-top: 80px;
}
.visual-subtitle {
  margin-bottom: 30px;
  font-size: 12px;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  color: #69746f;
}
.ae-grid {
  display: grid;
  grid-template-columns: 1.5fr 1fr 1fr;
  gap: 20px;
  align-items: start;
}
.ae-item {
  overflow: hidden;
  background: #dce2dd;
}
.ae-item:nth-child(1) {
  grid-row: span 2;
}
.ae-item img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
/* POSTERS */
.poster-wrapper {
  margin-top: 100px;
}
.poster-grid {
  display: grid;
  grid-template-columns: 1.1fr 0.9fr;
  gap: 25px;
  align-items: start;
}
.poster-column {
  display: flex;
  flex-direction: column;
  gap: 25px;
}
.poster-item {
  position: relative;
  overflow: hidden;
  background: #dce2dd;
}
.poster-item img {
  transition: transform 0.6s ease;
}
.poster-item:hover img {
  transform: scale(1.025);
}
.poster-label {
  padding: 14px 5px 5px;
  font-size: 11px;
  line-height: 1.7;
  color: #69746f;
}
/* =========================================================
   HIDE PAGE PAGINATION
   ========================================================= */
.portfolio-page + .page__pagination,
.page__pagination {
  display: none !important;
}
/* =========================================================
   MOBILE
   ========================================================= */
@media screen and (max-width: 900px) {
  .portfolio-page {
    padding: 10px 0 60px;
  }
  .portfolio-section {
    margin-bottom: 90px;
  }
  .portfolio-cover {
    min-height: auto;
    grid-template-columns: 1fr;
    gap: 45px;
    padding: 20px 0 70px;
  }
  .portfolio-cover-title {
    font-size: 82px;
  }
  .portfolio-cover-image {
    aspect-ratio: 4 / 5;
  }
  .copy-grid,
  .campaign-grid,
  .video-grid,
  .case-header,
  .case-images,
  .poster-grid {
    grid-template-columns: 1fr;
  }
  .social-layout {
    min-height: auto;
  }
  .social-main {
    width: 88%;
  }
  .social-secondary {
    position: relative;
    width: 58%;
    margin: -100px 0 0 auto;
  }
  .case-process {
    grid-template-columns: 1fr 1fr;
  }
  .ae-grid {
    grid-template-columns: 1fr 1fr;
  }
  .ae-item:nth-child(1) {
    grid-column: span 2;
    grid-row: auto;
  }
}
@media screen and (max-width: 600px) {
  .portfolio-cover-title {
    font-size: 62px;
  }
  .copy-card {
    min-height: 360px;
    padding: 30px;
  }
  .copy-card-title {
    margin-top: 45px;
    font-size: 28px;
  }
  .copy-card-info {
    left: 30px;
    bottom: 25px;
  }
  .case-process {
    grid-template-columns: 1fr;
  }
  .ae-grid {
    grid-template-columns: 1fr;
  }
  .ae-item:nth-child(1) {
    grid-column: auto;
  }
}
/* =========================================================
   PAGE BACKGROUND
   ========================================================= */
body {
  background:
    linear-gradient(
      135deg,
      rgba(216,230,220,0.72) 0%,
      rgba(250,250,246,0.9) 48%,
      rgba(241,220,226,0.62) 100%
    );
}
</style>
<div class="portfolio-page">
<!-- =====================================================
     01 / COVER
     ===================================================== -->
<section class="portfolio-section portfolio-cover">
  <div class="portfolio-cover-text">
    <div class="portfolio-cover-number">
      01 / PORTFOLIO
    </div>
    <h1 class="portfolio-cover-title">
      PORT<br>FOLIO
    </h1>
    <div class="portfolio-cover-name">
      杨芳个人作品集
    </div>
    <div class="portfolio-cover-role">
      文案编辑 / 策划 / 内容创作
    </div>
    <div class="portfolio-cover-meta">
      2022 — 2024<br>
      吉林大学 · 广告学
    </div>
  </div>
  <div class="portfolio-cover-image">
    <img
      src="/assets/images/portfolio/cover.jpg"
      alt="Portfolio Cover">
  </div>
</section>
<!-- =====================================================
     02 / COPY & CAMPAIGN
     ===================================================== -->
<section class="portfolio-section">
  <div class="portfolio-section-label">
    02 / COPY & CAMPAIGN
  </div>
  <h2 class="portfolio-section-title">
    文案与策划
  </h2>
  <p class="portfolio-section-description">
    从广告文案到策划案，再到新媒体内容，
    以文字作为创意起点，将策略转化为可执行的内容。
  </p>
  <!-- AD COPY -->
  <div class="campaign-title">
    AD COPY / 广告文案
  </div>
  <div class="copy-grid">
    <!-- 毓婷 -->
    <article class="copy-card">
      <div class="copy-card-number">
        01 / AD COPY
      </div>
      <h3 class="copy-card-title">
        毓婷
      </h3>
      <div class="copy-card-copy">
        很紧急，<br>
        用毓婷。
      </div>
      <div class="copy-card-info">
        中国大学生广告艺术节学院奖<br>
        2024 春季征集大赛优秀奖<br>
        命题企业：华润紫竹 · 毓婷
      </div>
    </article>
    <!-- 雅客 -->
    <article class="copy-card">
      <div class="copy-card-number">
        02 / AD COPY
      </div>
      <h3 class="copy-card-title">
        雅客
      </h3>
      <div class="copy-card-copy">
        从产品洞察出发，<br>
        将品牌信息转化为具有传播力的文字表达。
      </div>
      <div class="copy-card-info">
        中国大学生广告艺术节学院奖<br>
        2023 秋季征集大赛优秀奖<br>
        命题企业：雅客
      </div>
    </article>
  </div>
  <!-- CAMPAIGN -->
  <div class="campaign-wrapper">
    <div class="campaign-title">
      CAMPAIGN / 策划案
    </div>
    <div class="campaign-grid">
      <!-- 白象 -->
      <article class="campaign-card">
        <img
          src="/assets/images/portfolio/campaign-baixiang.jpg"
          alt="白象方便面策划案">
        <div class="campaign-card-info">
          <div class="campaign-card-number">
            01 / CAMPAIGN
          </div>
          <div class="campaign-card-name">
            白象方便面
          </div>
          <div class="campaign-card-description">
            从品牌与产品特征出发进行传播策划，
            将洞察、创意与传播执行连接起来。
          </div>
        </div>
      </article>
      <!-- 三顿半 -->
      <article class="campaign-card">
        <img
          src="/assets/images/portfolio/campaign-sannianban.jpg"
          alt="三顿半策划案">
        <div class="campaign-card-info">
          <div class="campaign-card-number">
            02 / CAMPAIGN
          </div>
          <div class="campaign-card-name">
            三顿半
          </div>
          <div class="campaign-card-description">
            品牌策划作品。
            重点呈现品牌洞察、创意方向与内容表达。
          </div>
        </div>
      </article>
    </div>
  </div>
  <!-- SOCIAL -->
  <div class="social-wrapper">
    <div class="social-title">
      SOCIAL / 新媒体
    </div>
    <div class="social-layout">
      <div class="social-main">
        <img
          src="/assets/images/portfolio/social-01.jpg"
          alt="影像传播实践作品">
        <div class="social-caption">
          影像传播实践课程作品 ·《此时。彼刻》
        </div>
      </div>
      <div class="social-secondary">
        <img
          src="/assets/images/portfolio/social-02.jpg"
          alt="影像传播实践作品">
        <div class="social-caption">
          影像传播实践课程作品 ·《此时。彼刻》
        </div>
      </div>
    </div>
  </div>
</section>
<!-- =====================================================
     03 / VIDEO
     ===================================================== -->
<section class="portfolio-section">
  <div class="portfolio-section-label">
    03 / VIDEO
  </div>
  <h2 class="portfolio-section-title">
    视频作品
  </h2>
  <p class="portfolio-section-description">
    从创意落地、分镜脚本、拍摄，到剪辑、调色与封装，
    参与不同类型的视频内容生产。
  </p>
  <div class="video-grid">
    <!-- 娃哈哈 -->
    <article class="video-card">
      <div class="video-media">
        <img
          src="/assets/images/portfolio/video-wahaha.jpg"
          alt="娃哈哈 AD钙奶 视频作品">
      </div>
      <div class="video-card-info">
        <div class="video-card-number">
          01 / VIDEO
        </div>
        <div class="video-card-title">
          娃哈哈 AD钙奶
        </div>
        <div class="video-card-description">
          《一滴千斤、记忆千金》<br>
          负责创意落地、分镜头脚本、拍摄、
          剪辑、调色与封装。
        </div>
      </div>
    </article>
    <!-- 讯飞星火 -->
    <article class="video-card">
      <div class="video-media">
        <img
          src="/assets/images/portfolio/video-xunfei.jpg"
          alt="讯飞星火 视频作品">
      </div>
      <div class="video-card-info">
        <div class="video-card-number">
          02 / VIDEO
        </div>
        <div class="video-card-title">
          讯飞星火
        </div>
        <div class="video-card-description">
          《金牌调解》<br>
          主要负责项目的剪辑与封装。
        </div>
      </div>
    </article>
    <!-- 启达力 -->
    <article class="video-card">
      <div class="video-media">
        <img
          src="/assets/images/portfolio/video-qidali.jpg"
          alt="启达力 视频作品">
      </div>
      <div class="video-card-info">
        <div class="video-card-number">
          03 / VIDEO
        </div>
        <div class="video-card-title">
          启达力
        </div>
        <div class="video-card-description">
          学院奖短视频作品。<br>
          从前期产品调研、创意生成、脚本撰写，
          到视频拍摄与剪辑制作。
        </div>
      </div>
    </article>
  </div>
</section>
<!-- =====================================================
     04 / FEATURED CASE
     ===================================================== -->
<section class="portfolio-section">
  <div class="portfolio-section-label">
    04 / FEATURED CASE
  </div>
  <div class="featured-case">
    <div class="case-header">
      <div class="case-header-title">
        启达力<br>
        短视频
      </div>
      <div class="case-header-description">
        以一个完整项目的方式，
        展示从前期研究到最终视频成片的工作流程。
        <br><br>
        这个案例重点呈现的不只是最终作品，
        而是从问题、创意、脚本到执行的完整过程。
      </div>
    </div>
    <!-- CASE COVER -->
    <div class="case-cover">
      <img
        src="/assets/images/portfolio/video-qidali.jpg"
        alt="启达力短视频">
      <div class="case-cover-label">
        QIDALI / SHORT VIDEO
      </div>
    </div>
    <!-- PROCESS -->
    <div class="case-process">
      <div class="case-process-item">
        <div class="case-process-number">
          01
        </div>
        <div class="case-process-title">
          Research
        </div>
        <div class="case-process-text">
          前期产品调研，梳理产品特征、
          使用场景与传播切入点。
        </div>
      </div>
      <div class="case-process-item">
        <div class="case-process-number">
          02
        </div>
        <div class="case-process-title">
          Idea
        </div>
        <div class="case-process-text">
          根据产品信息进行创意生成，
          确定视频内容方向。
        </div>
      </div>
      <div class="case-process-item">
        <div class="case-process-number">
          03
        </div>
        <div class="case-process-title">
          Script
        </div>
        <div class="case-process-text">
          将创意转化为完整脚本，
          设计人物、情节与画面。
        </div>
      </div>
      <div class="case-process-item">
        <div class="case-process-number">
          04
        </div>
        <div class="case-process-title">
          Production
        </div>
        <div class="case-process-text">
          完成视频拍摄，
          将前期创意转化为实际画面。
        </div>
      </div>
      <div class="case-process-item">
        <div class="case-process-number">
          05
        </div>
        <div class="case-process-title">
          Editing
        </div>
        <div class="case-process-text">
          完成剪辑、节奏控制、
          画面处理与最终成片。
        </div>
      </div>
    </div>
    <!-- CASE IMAGES -->
    <div class="case-images">
      <div class="case-image">
        <img
          src="/assets/images/portfolio/qidali-research.jpg"
          alt="启达力前期产品调研">
      </div>
      <div class="case-image">
        <img
          src="/assets/images/portfolio/qidali-script.jpg"
          alt="启达力脚本">
      </div>
      <div class="case-image">
        <img
          src="/assets/images/portfolio/qidali-production.jpg"
          alt="启达力视频拍摄">
      </div>
      <div class="case-image">
        <img
          src="/assets/images/portfolio/qidali-editing.jpg"
          alt="启达力视频剪辑">
      </div>
    </div>
  </div>
</section>
<!-- =====================================================
     05 / VISUAL
     ===================================================== -->
<section class="portfolio-section">
  <div class="portfolio-section-label">
    05 / VISUAL
  </div>
  <h2 class="portfolio-section-title">
    视觉设计
  </h2>
  <p class="portfolio-section-description">
    视觉设计作为文案与策划之外的执行能力，
    包括 AE 动效、平面广告、AI 视觉与公益广告。
  </p>
  <!-- AE -->
  <div class="visual-ae">
    <div class="visual-subtitle">
      COMPUTER DESIGN COMPETITION / AE
    </div>
    <div class="ae-grid">
      <div class="ae-item">
        <img
          src="/assets/images/portfolio/visual-ae-01.jpg"
          alt="计算机设计大赛 AE 作品">
      </div>
      <div class="ae-item">
        <img
          src="/assets/images/portfolio/visual-ae-02.jpg"
          alt="AE 动效设计">
      </div>
      <div class="ae-item">
        <img
          src="/assets/images/portfolio/visual-ae-03.jpg"
          alt="AE 动效设计">
      </div>
      <div class="ae-item">
        <img
          src="/assets/images/portfolio/visual-ae-04.jpg"
          alt="AE 动效设计">
      </div>
    </div>
  </div>
  <!-- POSTERS -->
  <div class="poster-wrapper">
    <div class="visual-subtitle">
      SELECTED POSTERS / 平面作品
    </div>
    <div class="poster-grid">
      <!-- LEFT -->
      <div class="poster-column">
        <div class="poster-item">
          <img
            src="/assets/images/portfolio/poster-yuting.jpg"
            alt="毓婷 很紧急 用毓婷">
          <div class="poster-label">
            毓婷 ·「很紧急，用毓婷」
          </div>
        </div>
        <div class="poster-item">
          <img
            src="/assets/images/portfolio/poster-blind.jpg"
            alt="禁止占用盲道公益广告">
          <div class="poster-label">
            公益广告 · 禁止占用盲道
          </div>
        </div>
      </div>
      <!-- RIGHT -->
      <div class="poster-column">
        <div class="poster-item">
          <img
            src="/assets/images/portfolio/poster-aihuashi.jpg"
            alt="爱华仕 AI 平面广告">
          <div class="poster-label">
            爱华仕 · AI 视觉广告
          </div>
        </div>
        <div class="poster-item">
          <img
            src="/assets/images/portfolio/poster-drunk-driving.jpg"
            alt="酒驾主题公益海报">
          <div class="poster-label">
            智能媒体大赛 · 酒驾主题
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
<!-- =====================================================
     END
     ===================================================== -->
<div style="
  padding-top:80px;
  border-top:1px solid rgba(31,39,36,0.18);
  font-size:11px;
  letter-spacing:0.16em;
  color:#78827d;
">
  YANG FANG / PORTFOLIO / 2022—2024
</div>
</div>

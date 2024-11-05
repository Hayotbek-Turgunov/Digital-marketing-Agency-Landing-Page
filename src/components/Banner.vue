<template>
  <section class="banner">
    <div class="container">
      <div class="banner-wrapper">
        <div class="banner-info">
          <h1 class="banner-info-title">
            Stay ahead of the curve with our forward-thinking
          </h1>
          <p class="banner-info-deck">
            An award-winning SEO agency with disciplines in digital marketing,
            design, and website development. focused on understanding you.
          </p>

          <div class="banner-btn-wrapper">
            <button class="button banner-btn">
              <span>Schedule Call</span>
              <span>
                <img :src="bannerBtnImg" alt="Header Logo" />
              </span>
            </button>

            <a class="banner-btn-link" href="">View Case Study</a>
          </div>

          <div class="banner-info-trusted">
            <p class="banner-info-trusted-title">
              Trusted by the world's biggest brands
            </p>

            <img :src="bannerTrustAfterpay" alt="Banner afterpay" />
            <img :src="bannerTrustBasecamp" alt="Banner basecamp" />
            <img :src="bannerTrustMaze" alt="Banner maze" />
          </div>
        </div>

        <div class="banner-statistics">
          <div class="banner-statistics-logo-count-wrapper">
            <div class="banner-statistics-logo">
              <div class="banner-statistics-logo-icon">
                <img :src="trandingUp" alt="Trending up" />
              </div>
            </div>
            <div class="banner-statistics-count">
              <h2 class="banner-statistics-count-title">230+</h2>
              <p class="banner-statistics-count-deck">
                some big companies that we work with, and trust us very much
              </p>
            </div>
          </div>

          <div class="banner-statistics-traffic">
            <img :src="bannerStatistics" alt="banner statistics" />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import bannerBtnImg from "../assets/icons/arrow-right.svg";
import bannerTrustAfterpay from "../assets/img/banner-afterpay.jpg";
import bannerTrustBasecamp from "../assets/img/banner-basecamp.jpg";
import bannerTrustMaze from "../assets/img/banner-maze.jpg";
import trandingUp from "../assets/icons/trending-up.svg";
import bannerStatistics from "../assets/img/banner-statistics.jpg";
</script>

<style lang="scss" scoped>
.banner {
  padding-top: 53px;

  &-wrapper {
    display: flex;

    .banner-info {
      width: 650px;

      &-title {
        font-family: Plus Jakarta Sans;
        font-size: 72px;
        font-weight: 600;
        line-height: 79.2px;
        letter-spacing: -0.03em;
        text-align: left;
        margin-bottom: 48px;
        width: 700px;
        height: 212px;
        gap: 0px;
        opacity: 0px;
      }

      &-deck {
        font-family: Plus Jakarta Sans;
        font-size: var(--font-size-small);
        font-weight: 500;
        line-height: 28.8px;
        text-align: left;
        color: var(--secondary-color);
        width: 557px;
        margin-bottom: 48px;
      }

      .banner-btn-wrapper {
        display: flex;
        align-items: center;
        gap: 56px;
        margin-bottom: 94px;

        .banner-btn {
          display: flex;
          align-items: center;
          background-color: var(--background-color);
          color: white;
          font-family: Plus Jakarta Sans;
          font-weight: 700;
          gap: 42px;

          & span {
            display: flex;
          }
        }

        .banner-btn-link {
          font-family: Plus Jakarta Sans;
          font-weight: 600;
          line-height: 28.8px;
          text-align: left;
          color: var(--text-color);
        }
      }

      &-trusted {
        display: flex;
        flex-wrap: wrap;
        align-items: center;
        gap: 28px;
        margin-bottom: 104px;

        &-title {
          font-family: Plus Jakarta Sans;
          // font-size: var(--font-size-small);
          font-size: 14px;
          font-weight: 600;
          line-height: 22.4px;
          text-align: left;
          width: 150px;
          margin-right: 60px;
        }
      }
    }

    .banner-statistics {
      display: flex;
      flex-direction: column;
      width: 588px;
      margin-top: 50px;

      &-logo-count-wrapper {
        display: flex;
        gap: 24px;
        margin-bottom: 24px;
      }

      &-logo {
        width: 303px;
        height: 275px;
        gap: 0px;
        border-radius: 1000px 20px 20px 20px;
        opacity: 0px;
        background-color: #00000033;
        &-icon {
          position: relative;
          width: 108px;
          height: 108px;
          border-radius: 50%;
          top: -40px;
          left: 150px;
          gap: 0px;
          opacity: 0px;
          background-color: black;
          display: flex;
          align-items: center;
          justify-content: center;
          box-shadow: 0px 8px 16px rgba(0, 0, 0, 0.2);
        }
      }

      &-count {
        width: 259px;
        height: 281px;
        border-radius: 20px 0px 0px 0px;
        opacity: 0px;
        background-color: #f0f0f0;
        border-radius: 20px;
        padding: 38px 25px;

        &-title {
          font-family: Plus Jakarta Sans;
          font-size: 84px;
          font-weight: 700;
          line-height: 126px;
          letter-spacing: -0.03em;
          text-align: left;
        }

        &-deck {
          font-family: Plus Jakarta Sans;
          color: #5c5d5f;
          font-weight: 500;
          line-height: 24px;
          text-align: left;
        }
      }
    }
  }
}
</style>

<template>
  <section class="services">
    <div class="container">
      <div class="services-head-wrappaer">
        <h2 class="services-head-title">
          Digital Marketing & SEO ServicesThat Grow Traffic & Increase Revenue
        </h2>

        <div class="services-head-right">
          <p class="services-head-deck">
            We are the top digital marketing agency for branding corp. We offer
            a full range of services to help clients improve their search engine
          </p>

          <button class="services-btn button">See more</button>
        </div>
      </div>

      <div class="services-cards">
        <div class="services-card">
          <div class="services-card-time">
            <div class="services-card-time-radius"></div>
            <p class="services-card-read-time">5 min read</p>
          </div>

          <h3 class="services-card-title">
            How a Digital Marketing Agency Can Boost Your Business
          </h3>

          <div class="services-deck-wrapper">
            <p class="services-deck">
              We are the top digital marketing agency for branding corp. We
              offer a full rang engine ....
            </p>
            <button class="services-deck-btn button">
              <span>
                <img :src="servicesArrowRight" alt="Services Arrow" />
              </span>
            </button>
          </div>
        </div>

        <div class="services-card">
          <div class="services-card-time">
            <div class="services-card-time-radius"></div>
            <p class="services-card-read-time">5 min read</p>
          </div>

          <h3 class="services-card-title">
            Maximizing ROI with the Expertise of a Digital Marketing Agency
          </h3>

          <div class="services-deck-wrapper">
            <p class="services-deck">
              Working with this digital marketing agency has been a true
              partnership.
            </p>
            <button class="service-secondary-btn button">
              <span>
                <img :src="servicesArrowRight2" alt="Services Arrow" />
              </span>
            </button>
          </div>
        </div>

        <div class="services-card">
          <div class="services-card-time">
            <div class="services-card-time-radius"></div>
            <p class="services-card-read-time">5 min read</p>
          </div>

          <h3 class="services-card-title">
            The Latest Trends and Strategies with a Digital Marketing Agency
          </h3>

          <div class="services-deck-wrapper">
            <p class="services-deck">
              What sets this digital marketing agency apart is their commitment
              to transparency y,
            </p>
            <button class="service-secondary-btn button">
              <span>
                <img :src="servicesArrowRight2" alt="Services Arrow" />
              </span>
            </button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import servicesArrowRight from "../assets/icons/arrow-right.svg";
import servicesArrowRight2 from "../assets/icons/arrow-right2.svg";
</script>

<style lang="scss" scoped>
.services {
  padding-top: 70px;
  margin-bottom: 127px;

  .services-head-wrappaer {
    display: flex;
    align-items: center;
    margin-bottom: 64px;

    .services-head-title {
      font-family: Plus Jakarta Sans;
      font-size: 48px;
      font-weight: 600;
      line-height: 62.4px;
      letter-spacing: -0.03em;
      text-align: left;
    }

    .services-head-deck {
      font-family: Plus Jakarta Sans;
      font-weight: 500;
      line-height: 28.8px;
      text-align: left;
      color: rgba(135, 140, 145, 1);
      margin-bottom: 48px;
    }

    .services-btn {
      padding: 17px 42px;
    }
  }

  .services-cards {
    display: flex;
    gap: 24px;

    .services-card {
      width: 410px;
      background-color: #2222221c;
      border-radius: 20px;
      padding: 32px;
      &-time {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 24px;

        .services-card-read-time {
          font-family: Plus Jakarta Sans;
          font-size: 14px;
          font-weight: 500;
          line-height: 22.4px;
          text-align: left;
        }

        &-radius {
          width: 14px;
          height: 14px;
          border-radius: 50%;
          background-color: rgba(69, 167, 222, 1);
        }
      }

      &-title {
        font-family: Plus Jakarta Sans;
        font-size: 26px;
        font-weight: 600;
        line-height: 39px;
        letter-spacing: -0.03em;
        text-align: left;
        margin-bottom: 56px;
      }

      .services-deck-wrapper {
        display: flex;
        align-items: center;
        gap: 38px;
      }

      .services-deck {
        font-family: Plus Jakarta Sans;
        font-size: 14px;
        font-weight: 500;
        line-height: 22.4px;
        text-align: left;
        color: rgba(135, 140, 145, 1);
      }

      .services-deck-btn {
        background-color: var(--background-color);
        border-radius: 70px;
        padding: 16px 32px;
      }

      .service-secondary-btn {
        background-color: white;
        padding: 16px 32px;
      }
    }
  }
}
</style>

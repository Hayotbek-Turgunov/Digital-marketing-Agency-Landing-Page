<template>
  <section class="testimonial">
    <div class="container">
      <h2 class="testimonial-title">
        “ They thoroughly analyze our industry and target audience, allowing
        them to develop customized campaigns that effectively reach and engage
        our customers. Their creative ideas and cutting-edge techniques have
        helped us stay ahead of the competition.”
      </h2>

      <div class="testimonial-view-profile">
        <div class="testimonial-view-profile-wrapper">
          <div class="testimonial-view-profile-img"></div>

          <div class="testimonial-profile-name-wrapper">
            <h3 class="testimonial-view-profile-name">Michael Kaizer</h3>
            <p class="testimonial-view-profile-title">CEO of Basecamp Corp</p>
          </div>
        </div>

        <div class="testimonial-view-button-wrapper">
          <button class="button testimonial-view-button-left">
            <span>
              <img :src="testimonialBtnImgLeft" alt="project  play" />
            </span>
          </button>
          <span class="testimonial-view-button-count">01/05</span>
          <button class="button testimonial-view-button-right">
            <img :src="testimonialBtnImgRight" alt="project  play" />
          </button>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import testimonialBtnImgRight from "../assets/icons/arrow-right.svg";
import testimonialBtnImgLeft from "../assets/icons/arrow-left.svg";
</script>

<style lang="scss" scoped>
.testimonial {
  &-title {
    font-family: Plus Jakarta Sans;
    font-size: 36px;
    font-weight: 600;
    line-height: 57.6px;
    letter-spacing: -0.03em;
    text-align: left;
    margin-bottom: 74px;
  }

  &-view-profile {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 74px;

    &-wrapper {
      display: flex;
      align-items: center;
      gap: 24px;

      .testimonial-view-profile-img {
        width: 70px;
        height: 70px;
        border-radius: 50%;
        background-color: rgba(0, 0, 0, 0.2);
      }

      .testimonial-view-profile-name {
        font-family: Plus Jakarta Sans;
        font-size: 20px;
        font-weight: 700;
        line-height: 36px;
        text-align: left;
      }

      .testimonial-view-profile-title {
        font-family: Plus Jakarta Sans;
        font-size: 16px;
        font-weight: 500;
        line-height: 28.8px;
        text-align: left;
        color: rgba(135, 140, 145, 1);
      }
    }

    .testimonial-view-button-wrapper {
      display: flex;
      align-items: center;
      gap: 38px;

      .testimonial-view-button-count {
        font-family: Plus Jakarta Sans;
        font-weight: 600;
        line-height: 28.8px;
        text-align: left;
      }

      .testimonial-view-button-right {
        background-color: var(--background-color);
      }
    }
  }
}
</style>

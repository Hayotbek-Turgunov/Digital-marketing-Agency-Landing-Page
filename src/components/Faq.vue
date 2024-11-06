<template>
  <section class="faq">
    <div class="faq-wrapper">
      <div class="faq-info">
        <h2 class="faq-info-title">Digital Marketing FAQs</h2>
        <p class="faq-info-deck">
          As a leading digital marketing agency, we are dedicated to providing
          comprehensive educational resources and answering frequently asked
          questions to help our clients.
        </p>
        <div class="faq-info-btn-wrapper">
          <button class="button faq-info-btn">More Questions</button>
          <a class="button-info-link" href="">Contact Us</a>
        </div>
      </div>

      <div class="faq-question">
        <div class="faq-question-item">
          <div class="faq-title-btn-wrapper">
            <h3 class="faq-qustion-item-title">
              Why is digital marketing important for my business?
            </h3>
            <button class="faq-question-item-btn">
              <span>
                <img :src="faqQuestionMinus" alt="project  play" />
              </span>
            </button>
          </div>
          <p class="faq-question-item-deck">
            Digital marketing allows businesses to reach and engage with a wider
            audience, generate leads, drive website traffic, and increase brand
            visibility. It provides measurable results, allows for targeted
            marketing efforts, and enables businesses to adapt and optimize
            their strategies based on data and insights.
          </p>
        </div>

        <div class="faq-question-item">
          <div class="faq-title-btn-wrappers">
            <h3 class="faq-qustion-item-titles">
              How can digital marketing help improve my website's visibility?
            </h3>
            <button class="faq-question-item-btn">
              <span>
                <img :src="faqQuestionPlus" alt="project  play" />
              </span>
            </button>
          </div>
        </div>

        <div class="faq-question-item">
          <div class="faq-title-btn-wrappers">
            <h3 class="faq-qustion-item-titles">
              How long does it take to see results from digital marketing
              efforts?
            </h3>
            <button class="faq-question-item-btn">
              <span>
                <img :src="faqQuestionPlus" alt="project  play" />
              </span>
            </button>
          </div>
        </div>

        <div class="faq-question-item">
          <div class="faq-title-btn-wrappers">
            <h3 class="faq-qustion-item-titles">
              How do you measure the success of digital marketing campaigns?
            </h3>
            <button class="faq-question-item-btn">
              <span>
                <img :src="faqQuestionPlus" alt="project  play" />
              </span>
            </button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import faqQuestionMinus from "../assets/icons/minus.svg";
import faqQuestionPlus from "../assets/icons/plus.svg";
</script>

<style lang="scss" scoped>
.faq {
  width: 1406px;
  height: 732px;

  border-radius: 28px;
  margin: auto;
  padding: 66px 80px;

  &-wrapper {
    display: flex;
    gap: 90px;

    .faq-info {
      width: 531px;
      height: 258px;

      &-title {
        font-family: Plus Jakarta Sans;
        font-size: var(--font-size-medium);
        font-weight: 600;
        line-height: 62.4px;
        letter-spacing: -0.03em;
        text-align: left;
        margin-bottom: 48px;
      }

      &-deck {
        font-family: Plus Jakarta Sans;
        font-weight: 500;
        line-height: 28.8px;
        text-align: left;
        color: rgba(135, 140, 145, 1);
        margin-bottom: 48px;
      }

      .faq-info-btn-wrapper {
        display: flex;
        align-items: center;
        gap: 48px;

        .faq-info-btn {
          padding: 17px 28px;
        }

        .button-info-link {
          font-family: Plus Jakarta Sans;
          color: var(--text-color);
          font-weight: 600;
          line-height: 28.8px;
          text-align: left;
        }
      }
    }

    .faq-question {
      width: 627px;
      height: 600px;
      &-item {
        border-top: 1px solid var(--text-color);
        border-bottom: 1px solid var(--text-color);
        padding-top: 26px;
        padding-bottom: 26px;

        .faq-title-btn-wrappers {
          display: flex;
          align-items: center;
          justify-content: space-between;
          .faq-qustion-item-titles {
            font-family: Plus Jakarta Sans;
            font-size: 24px;
            font-weight: 600;
            line-height: 36px;
            letter-spacing: -0.03em;
            text-align: left;
          }

          .faq-question-item-btn {
            border: none;
            background-color: inherit;
          }
        }

        .faq-title-btn-wrapper {
          display: flex;
          align-items: center;
          justify-content: space-between;
          margin-bottom: 48px;

          .faq-qustion-item-title {
            font-family: Plus Jakarta Sans;
            font-size: 24px;
            font-weight: 600;
            line-height: 36px;
            letter-spacing: -0.03em;
            text-align: left;
          }

          .faq-question-item-btn {
            border: none;
            background-color: inherit;
            cursor: pointer;

            & span {
              display: flex;
            }
          }
        }
        .faq-question-item-deck {
          font-family: Plus Jakarta Sans;
          font-weight: 500;
          line-height: 28.8px;
          text-align: left;
          color: rgba(135, 140, 145, 1);
        }
      }
    }
  }
}
</style>

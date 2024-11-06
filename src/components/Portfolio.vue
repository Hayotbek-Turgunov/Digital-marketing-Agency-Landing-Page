<template>
  <section class="portfolio">
    <h2 class="portfolio-head">
      Real-world examples of how we have helped companies achieve their
      marketing objectives.
    </h2>

    <div class="portfolio-filter-wrapper">
      <button class="button portfolio-filter-btn">All Work [20]</button>
      <button class="button portfolio-filter-btn portfolio-secondary-btn">
        UI/UX Design[10]
      </button>
      <button class="button portfolio-filter-btn">Digital Marketing [5]</button>
      <button class="button portfolio-filter-btn">Branding [5]</button>
    </div>

    <div class="portfolio-project-carts">
      <div class="project-cart project-cart-radius">
        <div class="project-cart-radius-item">
          <span>See Details</span>
        </div>
      </div>
      <div class="project-cart">
        <div class="project-cart-title-wrapper">
          <div class="project-card-title-line"></div>
          <p class="project-cart-title">Ai Corporation. 2023</p>
        </div>

        <h3 class="project-cart-deck">Ai Wave - Ai Chatbot Mobile App</h3>
      </div>
      <div class="project-cart">
        <div class="project-cart-title-wrapper">
          <div class="project-card-title-line"></div>
          <p class="project-cart-title">Lancer Corporation. 2023</p>
        </div>
        <h3 class="project-cart-deck">App Lancer - Freelance Mobile App</h3>
      </div>
    </div>
  </section>
</template>

<script setup>
import porfolioBoxBg from "../assets/img/project-box-bg2.png";
</script>

<style scoped lang="scss">
.portfolio {
  position: relative;
  width: 1380px;
  height: 900px;
  margin: auto;
  padding-left: 64px;
  // padding-right: 64px;
  padding-top: 80px;
  padding-bottom: 107px;
  background: url("../assets//img/project-box-bg2.png") no-repeat;
  background-size: cover;
  margin-bottom: 30px;
  border-radius: 30px;
  margin-bottom: 103px;

  &-head {
    text-align: center;
    font-family: Plus Jakarta Sans;
    font-size: var(--font-size-medium);
    font-weight: 600;
    line-height: 62.4px;
    letter-spacing: -0.03em;
    color: #fff;
    margin-bottom: 53px;
    padding-right: 64px;
  }
  &-filter-wrapper {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 24px;
    margin-bottom: 80px;
    padding-right: 64px;
  }

  .portfolio-filter-btn {
    padding: 13px 70px;
    font-family: Manrope;
    font-weight: 700;
    line-height: 22.4px;
    letter-spacing: -0.02em;
    text-align: left;
    background-color: black;
    color: white;
    border: 1px solid white;
  }

  .portfolio-secondary-btn {
    background-color: #99cf63;
  }

  &-project-carts {
    display: flex;
    gap: 40px;

    .project-cart {
      width: 420px;
      height: 420px;
      border: 11px solid gray;
      background-color: rgba(255, 255, 255, 0.7);
      border-radius: 10px;
      padding-top: 32px;
      padding-bottom: 41px;
      padding-left: 32px;
      display: flex;
      flex-direction: column;
      justify-content: space-between;

      &-title-wrapper {
        display: flex;
        align-items: center;
        gap: 13px;

        .project-cart-title {
          font-family: Plus Jakarta Sans;
          font-size: 17px;
          font-weight: 600;
          line-height: 21.42px;
          letter-spacing: -0.03em;
          text-align: left;
          color: rgba(255, 255, 255, 1);
        }

        .project-card-title-line {
          width: 54px;
          height: 1px;
          background-color: white;
        }
      }
      .project-cart-deck {
        font-family: Plus Jakarta Sans;
        font-size: 20px;
        font-weight: 600;
        line-height: 33.6px;
        text-align: left;
        color: rgba(255, 255, 255, 1);
      }
    }
    .project-cart-radius {
      border-radius: 50%;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 0;

      &-item {
        width: 163px;
        height: 163px;
        border-radius: 50%;
        background-color: rgba(153, 234, 72, 1);
        display: flex;
        align-items: center;
        justify-content: center;
        font-family: Plus Jakarta Sans;
        font-size: 18px;
        font-weight: 700;
        line-height: 22.68px;
        letter-spacing: -0.03em;
      }
    }
  }
}
</style>

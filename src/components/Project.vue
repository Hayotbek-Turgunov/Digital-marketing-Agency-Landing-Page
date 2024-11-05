<template>
  <section class="project">
    <div class="container">
      <div class="project-wrapper">
        <div class="project-count-box">
          <h3 class="project-count-box-count">920</h3>
          <p class="project-count-box-title">Project finish with superbly</p>

          <div class="project-count-bottom-wrapper">
            <div class="project-count-bottom-radius"></div>
            <div class="project-count-bottom-radius"></div>
            <div class="project-count-bottom-radius"></div>
            <div class="project-count-bottom-radius"></div>
            <a class="project-count-bottom-btn">
              <span>
                <img :src="projectBoxPlus" alt="project box plus" />
              </span>
            </a>
          </div>
        </div>
        <div class="project-count-work">
          <p class="project-count-work-title">HOW WE WORK</p>
          <button class="project-count-work-play">
            <span>
              <img :src="projectWorkPlay" alt="project  play" />
            </span>
          </button>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import projectBoxPlus from "../assets/icons/project-box-plus.svg";
import projectWorkPlay from "../assets/icons/project-play.svg";
</script>

<style lang="scss" scoped>
.project {
  margin-bottom: 90px;

  &-wrapper {
    display: flex;
    gap: 24px;
  }

  &-count-box {
    width: 438px;
    height: 382px;
    background: url("../assets/img/project-box-bg2.png") no-repeat;
    background-size: cover;
    border-radius: 30px;
    padding-left: 40px;
    padding-top: 10px;
    &-count {
      font-family: "Plus Jakarta Sans", sans-serif;
      font-size: 84px;
      font-weight: 700;
      line-height: 126px;
      letter-spacing: -0.03em;
      text-align: left;
      color: white;
    }
    &-count::after {
      content: "+";
      color: rgba(0, 128, 0, 0.659);
      font-size: 90px;
    }

    &-title {
      font-family: "Plus Jakarta Sans", sans-serif;
      font-size: 19px;
      font-weight: 500;
      line-height: 32.3px;
      text-align: left;
      color: var(--secondary-color);
      margin-top: 0;
    }
    .project-count-bottom-wrapper {
      margin-top: 110px;
      display: flex;
      align-items: center;
      margin-bottom: auto;
      gap: 7px;
      .project-count-bottom-radius {
        width: 70px;
        height: 70px;
        background-color: #c6c6c6;
        border-radius: 50%;
      }

      .project-count-bottom-btn {
        border: none;
        background: inherit;
        cursor: pointer;
      }
    }
  }

  &-count-work {
    width: 818px;
    height: 382px;
    background-color: #00000033;
    border-radius: 30px;
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;

    &-title {
      font-family: Plus Jakarta Sans;
      font-size: 48px;
      font-weight: 600;
      line-height: 67.2px;
      letter-spacing: 0.27em;
      text-align: left;
      color: #fff;
    }

    &-play {
      width: 163px;
      height: 163px;
      background-color: #99ea48;
      border: 12px solid #fff;
      display: flex;
      align-items: center;
      justify-content: center;
      border-radius: 50%;
      position: absolute;
      bottom: -15px;
      right: -30px;
      cursor: pointer;

      & span {
        display: flex;
      }
    }
  }
}
</style>

<template>
  <section class="aside">
    <div class="aside-wrapper">
      <h2 class="aside-title">Ready to work with us ?</h2>
      <button class="aside-btn button">
        <span>Get Started</span>
        <span>
          <img :src="asideArrowRight2" alt="aside Arrow" />
        </span>
      </button>
    </div>
  </section>
</template>

<script setup>
import asideArrowRight2 from "../assets/icons/arrow-right2.svg";
</script>

<style scoped lang="scss">
.aside {
  width: 1400px;
  margin: auto;
  background-image: url("../assets/img//project-box-bg2.png");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  margin-bottom: 20px;
  border-radius: 30px;
  padding-left: 80px;
  padding-right: 117px;

  &-wrapper {
    height: 300px;
    display: flex;
    align-items: center;
    justify-content: space-between;

    .aside-title {
      font-family: Plus Jakarta Sans;
      font-size: 80px;
      font-weight: 600;
      line-height: 104px;
      letter-spacing: -0.03em;
      text-align: left;
      color: rgba(255, 255, 255, 1);
    }

    .aside-btn {
      display: flex;
      align-items: center;
      padding: 22px 32px;
      gap: 42px;

      & span {
        display: flex;
      }
    }
  }
}
</style>

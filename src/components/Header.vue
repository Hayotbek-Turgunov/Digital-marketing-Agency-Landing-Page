<template>
  <header>
    <div class="container">
      <div class="header-wrapper">
        <a class="header-link" href="#">
          <img :src="headerLogo" alt="Header Logo" />
          <span>MAC</span>
        </a>
        <nav class="header-nav">
          <ul class="header-nav-list">
            <li class="header-nav-list-item">
              <a class="header-nav-list-item-link" href=""
                >Service
                <span>
                  <img :src="headerListArrow" alt="Header List Arrow" />
                </span>
              </a>
            </li>
            <li class="header-nav-list-item">
              <a class="header-nav-list-item-link" href=""
                >Agency
                <span>
                  <img :src="headerListArrow" alt="Header List Arrow" />
                </span>
              </a>
            </li>
            <li class="header-nav-list-item">
              <a class="header-nav-list-item-link" href=""
                >Case study

                <span>
                  <img :src="headerListArrow" alt="Header List Arrow" />
                </span>
              </a>
            </li>
            <li class="header-nav-list -item">
              <a class="header-nav-list-item-link" href=""
                >Resources

                <span>
                  <img :src="headerListArrow" alt="Header List Arrow" />
                </span>
              </a>
            </li>
            <li class="header-nav-list-item">
              <a class="header-nav-list-item-link" href="">Contact </a>
            </li>
          </ul>
        </nav>

        <div class="header-btn-wrapper">
          <button class="header-btn button">Get started</button>
          <button class="header-btn-sound button">
            <span>
              <img :src="headerBtn" alt="Header Btn Sound" />
            </span>
          </button>
        </div>
      </div>
    </div>
  </header>
</template>

<script setup>
import headerLogo from "../assets/icons/header-logo.svg";
import headerListArrow from "../assets/icons/header-list-arrow.svg";
import headerBtn from "../assets/icons/header-btn-soung.svg";
</script>

<style lang="scss" scoped>
header {
  padding-top: var(--padding-medium);
  padding-bottom: var(--padding-medium);

  .header-wrapper {
    display: flex;
    align-items: center;

    .header-link {
      display: flex;
      align-items: center;
      justify-content: center;
      text-decoration: none;
      margin-right: 74px;
      gap: 8px;

      & img {
        width: 33px;
        height: 33px;
      }

      & span {
        font-family: Manrope;
        font-size: 24px;
        font-weight: 700;
        line-height: 32.78px;
        letter-spacing: -0.05em;
        text-align: left;
        color: var(--text-color);
      }
    }

    .header-nav {
      margin-right: auto;
      &-list {
        display: flex;
        align-items: center;
        list-style: none;
        gap: 33px;

        .header-nav-list-item-link {
          display: flex;
          align-items: center;
          font-family: Plus Jakarta Sans;
          font-size: var(--font-size-small);
          font-weight: 600;
          line-height: 17.64px;
          text-align: left;
          color: var(--text-color);
          text-decoration: none;
          gap: 7px;
        }
      }
    }

    .header-btn-wrapper {
      display: flex;
      gap: 9px;
      align-items: center;

      .header-btn-sound {
        background-color: var(--background-color);
        padding: 13px;
      }

      & span {
        display: flex;
      }
    }
  }
}
</style>

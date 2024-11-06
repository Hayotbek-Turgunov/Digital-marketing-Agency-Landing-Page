<template>
  <section class="footer">
    <div class="container">
      <div class="footer-wrapper">
        <div class="footer-item-info">
          <a class="footer-logo-link" href="#">
            <img :src="headerLogo" alt="Header Logo" />
            <span>MAC</span>
          </a>

          <p class="footer-item-info-deck">
            We offers a comprehensive suite of digital marketing services that
            cover all aspects of our online presence. From SEO and social media
            marketing to content creation and PPC advertising, they have the
            expertise and resources to handle our diverse marketing needs.
          </p>

          <div class="footer-item-info-social">
            <div class="footer-item-social-item">
              <img :src="footerSocialIconFa" alt="Header Logo" />
            </div>
            <div class="footer-item-social-item">
              <img :src="footerSocialIconTw" alt="Header Logo" />
            </div>
            <div class="footer-item-social-item">
              <img :src="footerSocialIconIn" alt="Header Logo" />
            </div>
            <div class="footer-item-social-item">
              <img :src="footerSocialIconInsta" alt="Header Logo" />
            </div>
          </div>
        </div>

        <div class="footer-item">
          <h2 class="footer-item-title">Navigation</h2>
          <ul class="footer-item-list">
            <li class="footer-list-item">
              <a href="">Service</a>
            </li>
            <li class="footer-list-item">
              <a href="">Agency</a>
            </li>
            <li class="footer-list-item">
              <a href="">Case Study</a>
            </li>
            <li class="footer-list-item">
              <a href="">Resource</a>
            </li>
            <li class="footer-list-item">
              <a href="">Contact</a>
            </li>
          </ul>
        </div>

        <div class="footer-item">
          <h2 class="footer-item-title">Licence</h2>
          <ul class="footer-item-list">
            <li class="footer-list-item">
              <a href="">Privacy Policy </a>
            </li>
            <li class="footer-list-item">
              <a href="">Copyright</a>
            </li>
            <li class="footer-list-item">
              <a href="">Email Address</a>
            </li>
          </ul>
        </div>

        <div class="footer-item">
          <h2 class="footer-item-title">Contact</h2>
          <ul class="footer-item-list">
            <li class="footer-list-item">
              <a href="">(406) 555-0120</a>
            </li>
            <li class="footer-list-item">
              <a href="">Hey@boostim.com</a>
            </li>
            <li class="footer-list-item">
              <a href="">2972 Westheimer Rd. Santa Ana, Illinois 85486 </a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import headerLogo from "../assets/icons/header-logo.svg";
import footerSocialIconFa from "../assets/icons/facebook.svg";
import footerSocialIconTw from "../assets/icons/twitter.svg";
import footerSocialIconIn from "../assets/icons/in.svg";
import footerSocialIconInsta from "../assets/icons/instagram logo.svg";
</script>

<style lang="scss" scoped>
.footer {
  margin-top: 90px;

  &-wrapper {
    display: flex;
    gap: 108px;
  }

  &-item-info {
    width: 534px;

    .footer-logo-link {
      display: flex;
      align-items: center;
      text-decoration: none;
      gap: 12px;
      margin-bottom: 30px;

      & img {
        width: 51px;
        height: 51px;
      }

      & span {
        font-family: Manrope;
        font-size: 37.09px;
        font-weight: 700;
        line-height: 50.67px;
        letter-spacing: -0.05em;
        text-align: left;
        color: var(--text-color);
      }
    }

    &-deck {
      font-family: Roboto;
      font-size: 14px;
      font-weight: 400;
      line-height: 24px;
      text-align: left;
      color: rgba(155, 155, 156, 1);
      margin-bottom: 30px;
    }

    &-social {
      display: flex;
      gap: 12px;

      .footer-item-social-item {
        width: 34px;
        height: 34px;
        border-radius: 50%;
        background-color: bisque;
        display: flex;
        align-items: center;
        justify-content: center;

        &-img {
          display: flex;
        }
      }
    }
  }

  .footer-item-title {
    font-family: Roboto;
    font-size: 18px;
    font-weight: 600;
    line-height: 21.09px;
    letter-spacing: -0.01em;
    text-align: left;
    margin-bottom: 40px;
  }

  .footer-list-item {
    margin-bottom: 20px;
  }

  .footer-item-list {
    list-style: none;

    & a {
      text-decoration: none;
      white-space: nowrap;
      font-family: Roboto;
      font-size: 14px;
      font-weight: 400;
      line-height: 16.41px;
      letter-spacing: -0.02em;
      text-align: left;
      color: rgba(155, 155, 156, 1);
    }
  }
}
</style>

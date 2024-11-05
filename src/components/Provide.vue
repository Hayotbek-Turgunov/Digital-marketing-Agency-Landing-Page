<template>
  <section class="provide">
    <div class="container">
      <div class="provide-wrapper">
        <div class="provide-left">
          <h2 class="provide-left-title">
            Provide the best service with out of the box ideas
          </h2>
        </div>

        <div class="provide-right">
          <h2 class="provide-right-title">
            we are a passionate team of digital marketing enthusiasts dedicated
            to helping businesses succeed in the digital world. With years of
            experience and a deep understanding of the ever-evolving online
            landscape, we stay at the forefront of industry trends and
            technologies.
          </h2>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.provide {
  margin-bottom: 72px;

  &-wrapper {
    display: flex;
    align-items: center;

    .provide-left {
      width: 684px;

      &-title {
        font-family: Plus Jakarta Sans;
        font-size: 48px;
        font-weight: 600;
        line-height: 62.4px;
        letter-spacing: -0.03em;
        text-align: left;
        width: 684px;
      }
    }

    .provide-right {
      width: 557px;

      &-title {
        font-family: Plus Jakarta Sans;
        font-weight: 500;
        line-height: 28.8px;
        text-align: left;
        color: var(--secondary-color);
      }
    }
  }
}
</style>

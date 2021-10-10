<template>
    <section class="welcome-section">
      <div class="container">
        <div class="left-side">
          <div class="bubble-wrapper-mobile">
            <div class="bubble-greeting-mobile">
              <h1 class="bubble-speech">Hi, this is Angela</h1>
            </div>
            <div class="bubble-trail">
              <img src="~/assets/svg/bubble-trail.svg" alt="">
            </div>
          </div>
          <div class="picture">
            <img src="angela-hello.gif" alt="angela-s-animoji">
          </div>
          <div class="speech-text">
            <h1 class="bubble-speech">Hi, this is Angela</h1>
            <h4>
              She works @an international, multicultural company in Germany, Karlsruhe - FIZ Karlsruhe. She likes to put pins on the map of each one of her colleagues’ nationality. Since the change WFO - WFH from Covid-19 regulations, she misses her map at the office.
            </h4>
          </div>
        </div>
        <div class="right-side">
          <!-- map image -->
        </div>
      </div>
    </section>
</template>
<style lang="scss" scoped>
// welcome section
section.welcome-section {
  width: 100%;
  height: calc(100vh - 80px);
  .left-side {
    width: 100%;
    display: flex;
    flex-direction: column;
    .bubble-wrapper-mobile {
      width: 100%;
      display: flex;
      justify-content: right;
      position: relative;
      .bubble-greeting-mobile {
        width: 292px;
        height: 95px;
        background: url('~/assets/svg/bubble.svg');
        display: flex;
        justify-content: center;
        align-items: center;
        margin-right: 20px;
      }
      .bubble-trail {
        position: absolute;
        bottom: 0; right: -292px;
      }
    }
    .picture {
      width: 245px;
      margin-left: 20px;
      img {
        width: 100%;
      }
    }
  }
}
</style>

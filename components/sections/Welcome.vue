<template>
    <section class="welcome-section">
      <div class="o-container">
        <div class="left-side">
          <div class="animoji-talking">
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
          </div>
          <div class="speech-text">
            <h4>
              She works @FIZ Karlsruhe, a multinational company.<br><br> She likes to put a pin on the countries of her fellow colleagues’ nationality.
            </h4>
          </div>
        </div>
        <div class="right-side">
          <div class="map-holder">
            <img src="/map-block.png" alt="map-block">
          </div>
          <Buttons-Primary />
        </div>
      </div>
    </section>
</template>
<style lang="scss" scoped>
// welcome section
section.welcome-section {
  width: 100%;
  min-height: calc(100vh - 80px);
  .o-container {
    @include mq($from: desktop) {
      display: flex;
      flex-direction: row;
      justify-content: space-between;
    }
  }
  .left-side {
    width: 100%;
    display: flex;
    flex-direction: column;
    @include mq($from: desktop) {
      width: 556px;
    }
    .animoji-talking {
      width: 100%;
      max-width: 500px;
      margin: auto;
    }
    .bubble-wrapper-mobile {
      width: 100%;
      max-width:556px;
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
        // bottom: 0; right: -292px; - desktop
        top: 80px; right: 310px;
      }
    }
    .picture {
      width: 245px;
      margin-left: 20px;
      margin-top: 20px;
      img {
        width: 100%;
      }
    }
    .speech-text {
      font-size: 22px;
    }
  }
  .right-side {
    width: 100%;
    max-width: 747px;
    overflow: hidden;
    margin-left: 24px;
    @include mq($from: desktop) {
      width: 747px;
      margin-right: -24px;
    }
    .map-holder {
      width: 100%;
      img {
        width: 100%;
      }
    }
  }
}
</style>

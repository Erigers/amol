<template>
    <section class="welcome-section">
      <div class="o-container">
        <div class="left-side">
          <div class="animoji-talking">
            <div class="picture">
              <div class="picture-stance">
                <img src="~/assets/svg/hi-angela-bckg.svg" alt="hi-angela-stance">
              </div>
              <img src="angela-hello.gif" alt="angela-s-animoji">
            </div>
            <div class="speech-text">
              <div class="bubble-wrapper-mobile">
                <div class="bubble-greeting-mobile">
                  <h1 class="bubble-speech">Hi, this is Angela</h1>
                </div>
                <div class="bubble-trail">
                  <img src="~/assets/svg/bubble-trail.svg" alt="bubble-trail">
                </div>
              </div>
              <h4>
                She works @FIZ Karlsruhe, a multinational company.<br><br> She likes to put a pin on the countries of her fellow colleagues’ nationality.
              </h4>
            </div>
          </div>
        </div>
        <div class="right-side">
          <div class="map-holder">
            <img src="/map-block.png" alt="map-block">
          </div>
          <Buttons-Primary />
          <div class="chevron-holder">
            <img src="~/assets/svg/chevrons-down.svg" alt="chevrons-down">
          </div>
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
    position: relative;
    @include mq($from: desktop) {
      width: 510px;
      flex-direction: row;
    }
    @include mq($from: wide) {
      width: 600px;
      margin-top: 100px;
    }
    .animoji-talking {
      width: 100%;
      max-width: 500px;
      margin: auto;
      @include mq($from: wide) {
        max-width: 600px;
        display: flex;
      }
      .picture {
        width: 245px;
        margin-left: 20px;
        margin-top: 110px;
        position: relative;
        img {
          position: relative;
          width: 100%;
          z-index: 2;
        }
        .picture-stance {
          position: absolute;
          bottom: -25px;
          z-index: 1;
        }
      }
      .speech-text {
        font-size: 22px;
        .bubble-wrapper-mobile {
          width: 100%;
          max-width: 556px;
          display: flex;
          justify-content: right;
          position: absolute;
          top: 0; left: 0;
          .bubble-greeting-mobile {
            width: 292px;
            height: 95px;
            background: url('~/assets/svg/bubble.svg');
            display: flex;
            justify-content: center;
            align-items: center;
            margin-right: 20px;
            h1 {
              font-size: 38px;
            }
          }
          .bubble-trail {
            position: absolute;
            // bottom: 0; right: -292px; - desktop
            top: 80px; right: 310px;
          }
        }
        h4 {
          @include mq($from: wide) {
            max-width: 330px;
            margin-top: 150px;
          }
        }
      }
    }
  }
  .right-side {
    width: 100%;
    max-width: 747px;
    overflow: hidden;
    @include mq($from: wide) {
      position: absolute;
      right: 0;
      top: 100px;
      max-width: 1000px;
      width: calc(100% - 700px);
    }
    .map-holder {
      width: 100%;
      @include mq($from: wide) {
        margin-right: -24px;
      }
      img {
        width: 100%;
      }
    }
    .button-holder {
      width: 355px;
      margin: auto;
      @include mq($from: phablet) {
        margin-top: -90px;
        margin-bottom: 90px;
      }
    }
    .chevron-holder {
      margin-top: -50px;
      cursor: pointer;
      transition: all .5s;
      animation-name: scrollDown;
      animation-duration: 2s;
      animation-iteration-count: infinite;
    }
  }
  @keyframes scrollDown {
    0% {
      margin-top: -50px;
    }
    50% {
      margin-top: -60px;
    }
    100% {
      margin-top: -50px;
    }
  }
}
</style>

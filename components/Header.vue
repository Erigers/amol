<template>
    <header class="header flex-center">
      <div class="o-container flex-space-between">
        <div class="logo-holder">
          <img src="~/assets/svg/amol-logo.svg" alt="amol-logo">
        </div>
        <div class="options flex-space-between">
          <div class="flag english-flag">
            <img src="~/assets/svg/english-flag.svg" alt="english-flag">
          </div>
          <div class="flag german-flag">
            <img src="~/assets/svg/german-flag.svg" alt="german-flag">
          </div>
          <img src="/Fixed.png" alt="google-login">
        </div>
      </div>
    </header>
</template>
<style lang="scss" scoped>
// Header
header {
  width: 100%;
  height: 130px;
  .logo-holder {
    width: 150px;
    height: 64px;
    @include mq($from: phablet) {
      width: 210px;
      height: 90px;
    }
    img {
      width: 100%;
    }
  }
  .options {
    width: 250px;
    @include mq($from: wide) {
      width: 350px;
    }
    .flag {
      width: 42px;
      height: 42px;
      border-radius: 50%;
      border: 5px solid transparent;
      overflow: hidden;
      transition: all .5s;
      cursor: pointer;
      &:hover {
        border: 5px solid $color-blue;
      }
      img {
        width: 100%;
        border-radius: 50%;
      }
    }
  }
  img {
    width: 150px;
    @include mq($from: wide) {
      width: 250px;
    }
  }
}
</style>

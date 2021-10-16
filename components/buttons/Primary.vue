<template>
  <div class="button-holder">
    <button class="flex-center">
      <img src="~/assets/svg/map-pin.svg" alt="pin-icon">
      Start Pinning
    </button>
    <div class="after-background" />
  </div>
</template>
<style lang="scss" scoped>
.button-holder {
  position: relative;
  width: 355px;
  margin: auto;
  margin-top: -90px;
  margin-bottom: 90px;
  .after-background {
    position: absolute;
    top: 10px;
    left: -10px;
    width: 355px;
    height: 50px;
    border-radius: 7px;
    border: 1px solid transparent;
    background: $color-tertiary;
    z-index: 1;
    transition: all .5s;
  }
}
button {
  position: relative;
  width: 355px;
  height: 50px;
  border-radius: 7px;
  border: 1px solid $color-dark;
  background: $color-white;
  font-family: $font-header;
  font-size: 28px;
  color: $color-dark;
  z-index: 2;
  cursor: pointer;
  transition: all .5s;
  &:hover {
    background: $color-light-grey;
  }
  &:hover + .after-background {
    top: 5px;
    left: -5px;
  }
}
</style>

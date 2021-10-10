<template>
    <header>
      <div class="container">
        <div class="logo-holder">
          <img src="~/assets/svg/amol-logo.svg" alt="amol-logo">
        </div>
        <div class="options">
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
  height: 120px;
  display: flex;
  align-items: center;
  justify-content: center;
  .container {
    max-width: 1440px;
    width: 90%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    .options {
      width: 329px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      .flag {
        width: 45px;
        height: 45px;
        border-radius: 50%;
        border: 5px solid transparent;
        overflow: hidden;
        transition: all .5s;
        cursor: pointer;
        &:hover {
          border: 5px solid #476CF2;
        }
        img {
          width: 100%;
        }
      }
    }
  }
  img {
    width: 200px;
  }
}
</style>

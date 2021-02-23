<template>
  <div class="header">
    <div class="header__nav">
      <div class="header__nav-item">Home</div>
      <div class="header__nav-item">About me</div>
      <div class="header__nav-item">Skills</div>
      <div class="header__nav-item">Portfolio</div>
      <div class="header__nav-item">Contacts</div>
    </div>
    <div class="header__line"></div>
  </div>
</template>

<style lang="scss" scoped>
.header {
  width: 80%;
  margin: 0 auto;
  &__nav {
    display: flex;
    justify-content: space-between;
    // display: grid;
    // grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
    // grid-template-rows: 30px;
    // margin: 2% -9%;
  }
  //   &__nav-item {
  //     text-align: center;
  //   }
  &__line {
    border-bottom: 2px solid black;
    width: 100%;
  }
}
</style>

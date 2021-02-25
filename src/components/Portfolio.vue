<template>
  <div class="portfolio">
    <div class="portfolio__title title">Portfolio</div>
    <div class="portfolio__item">
      <img src="@/assets/screen.png" />
      <p>here is link to smth</p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.portfolio {
  width: 100%;
  height: 2253px;
  background-color: rgba(246, 246, 246, 1);
  &__title {
    padding-top: 113px;
    text-align: center;
    margin-bottom: 47px;
  }
  &__item {
    display: flex;
    flex-direction: column;
    align-items: center;
    img {
      width: 80%;
      margin-bottom: 45px;
    }
  }
}
</style>

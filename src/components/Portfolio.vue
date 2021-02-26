<template>
  <div class="portfolio">
    <div class="portfolio__title title">Portfolio</div>
    <div class="portfolio__item">
      <img src="@/assets/thrive.png" />
      <a>here is link to smth</a>
    </div>
    <div class="portfolio__item">
      <img src="@/assets/thrive.png" />
      <a>here is link to smth</a>
    </div>
    <div class="portfolio__item">
      <img src="@/assets/thrive.png" />
      <a>here is link to smth</a>
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
    a {
      margin-bottom: 100px;
      &:hover {
        cursor: pointer;
      }
    }
  }
}
</style>

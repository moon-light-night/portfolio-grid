<template>
  <div class="portfolio">
    <div class="portfolio__title"><a name="portfolio">Portfolio</a></div>
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
@import '@/profile/mixins.scss';

.portfolio {
  width: 100%;
  padding: 113px 0 0 0;
  background-color: rgb(235, 223, 223);
  &__title {
    @include style_title;
    margin: 0 0 47px 0;
  }
  &__item {
    display: flex;
    flex-direction: column;
    align-items: center;
    img {
      width: 80%;
      margin: 0 0 45px;
    }
    a {
      margin: 0 0 99px;
      &:hover {
        cursor: pointer;
      }
    }
  }
}
</style>

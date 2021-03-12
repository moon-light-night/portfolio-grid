<template>
  <div class="footer__wrap">
    <div class="footer__content">
      <div class="footer__title">
        <a name="contacts">Contacts</a>
      </div>
      <div class="footer__description">
        Want to know more or just chat? You are welcome!
      </div>
      <a class="footer__btn">Send message</a>
      <div class="footer__links">
        <div class="footer__link">
          <svg class="svg-icon">
            <use xlink:href="#telegram"></use>
          </svg>
        </div>
        <div class="footer__link">
          <svg class="svg-icon">
            <use xlink:href="#github"></use>
          </svg>
        </div>
        <div class="footer__link">
          <svg class="svg-icon">
            <use xlink:href="#instagram"></use>
          </svg>
        </div>
      </div>
      <div class="footer__sub-description">
        Connect me on<br />
        Telegram, GitHub, Instagram
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@import '@/profile/mixins.scss';

.footer {
  &__wrap {
    width: 100%;
    padding: 114px 0 0 0;
  }
  &__content {
    width: 345px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  &__title {
    @include style_title;
    margin: 0 0 40px 0;
  }
  &__description {
    font-size: 18px;
    text-align: center;
    margin: 0 0 30px 0;
  }
  &__btn {
    width: 180px;
    height: 42px;
    background-color: black;
    color: white;
    border-radius: 26px;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0 0 85px 0;
    font-size: 18px;
    transition: 0.3s linear;
    &:hover {
      cursor: pointer;
      transform: scale(1.1);
      color: rgb(190, 12, 12);
    }
  }
  &__links {
    display: flex;
    justify-content: space-between;
    width: 100%;
    margin: 0 0 45px;
  }
  &__sub-description {
    padding: 0 50px;
    margin: 0 0 123px;
    text-align: center;
    font-size: 14px;
    color: rgba(130, 130, 130, 1);
  }
}
.svg-icon {
  width: 48px;
  height: 48px;
  transition: 0.3s linear;
  border-radius: 50%;
  &:hover {
    cursor: pointer;
    transform: scale(1.2);
    background-color: rgb(190, 12, 12);
  }
}
</style>

<template>
  <div>
    <div class="header__wrap">
      <div class="header__modal hide">
        <div class="header__modal-item1"><a href="#home">Home</a></div>
        <div class="header__modal-item2"><a href="#about">About me</a></div>
        <div class="header__modal-item3"><a href="#skills">Skills</a></div>
        <div class="header__modal-item4">
          <a href="#portfolio">Portfolio</a>
        </div>
        <div class="header__modal-item5"><a href="#contacts">Contacts</a></div>
        <div class="header__modal-item6">
          <img src="@/assets/close.png" alt="img" @click="getModal" />
        </div>
        <div class="header__modal-item7">RU | ENG</div>
      </div>
    </div>
    <div class="header__content">
      <div class="header__nav">
        <div class="header__nav-item"><a href="#home">Home</a></div>
        <div class="header__nav-item"><a href="#about">About me</a></div>
        <div class="header__nav-item"><a href="#skills">Skills</a></div>
        <div class="header__nav-item"><a href="#portfolio">Portfolio</a></div>
        <div class="header__nav-item"><a href="#contacts">Contacts</a></div>
      </div>
      <div class="header__line"></div>
      <div class="header__info">
        <div class="header__info-name">
          Ilya<br />
          Baskakov
        </div>
        <div class="header__info-icon" @click="getModal">
          <img src="@/assets/nav-icon.png" alt="img" />
        </div>
        <div class="header__info-desc">
          Fr. developer<br />21 y.o. Stavropol
        </div>
        <div class="header__info-lang">RU | ENG</div>
      </div>
      <div class="header__info-photo">
        <img src="@/assets/avatar.png" alt="img" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    getModal() {
      document.querySelector('.header__modal').classList.toggle('hide')
    },
  },
}
</script>

<style lang="scss" scoped>
@import '@/profile/variables.scss';
@import '@/profile/mixins.scss';

.header {
  &__wrap {
    width: 100%;
  }
  &__content {
    width: 90%;
    margin: 0 auto;
  }
  &__nav {
    @include style_text;
    display: flex;
    justify-content: space-between;
    margin: 30px 0;
    @media (max-width: 375px) {
      display: none;
    }
  }
  &__nav-item {
    &:hover {
      cursor: pointer;
    }
  }
  &__line {
    border-bottom: 2px solid black;
    width: 100%;
    margin: 30px 0;
    @media (max-width: 375px) {
      display: none;
    }
  }
  &__info {
    display: grid;
    grid-template-areas: 'name desc lang';
    @media (max-width: 375px) {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 20px;
      margin-top: 20px;
      grid-template-areas:
        'name icon'
        'desc .';
    }
  }
  &__info-name {
    @include style_title;
    text-align: left;
    line-height: 50px;
    grid-area: name;
    @media (max-width: 375px) {
      line-height: 30px;
    }
  }
  &__info-icon {
    display: none;
    grid-area: icon;
    @media (max-width: 375px) {
      display: flex;
      justify-self: right;
      align-self: flex-start;
      margin: 5px;
    }
    &:hover {
      cursor: pointer;
    }
  }
  &__info-desc {
    @include style_text;
    justify-self: center;
    align-self: center;
    text-align: center;
    grid-area: desc;
    padding-right: 90px;
    @media (max-width: 540px) {
      padding-right: 50px;
    }
    @media (max-width: 375px) {
      justify-self: start;
      text-align: left;
    }
  }
  &__info-lang {
    @include style_text;
    justify-self: end;
    align-self: center;
    grid-area: lang;
    transform: rotate(-90deg);
    margin-right: -25px;
    @media (max-width: 375px) {
      display: none;
    }
  }
  &__info-photo {
    display: flex;
    justify-content: center;
    margin: 50px 0;
    img {
      @media (max-width: 550px) {
        width: 100%;
      }
    }
  }
  &__modal {
    background-color: white;
    position: absolute;
    top: 0;
    width: 100%;
    height: 610px;
    font-size: 34px;
    line-height: 42px;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(6, 1fr);
    grid-template-areas:
      'name close' 'about about' 'skills skills' 'portfolio portfolio'
      'contacts contacts' '. lang';
    @media (min-width: $phone_sz) {
      display: none;
    }
  }
  &__modal-item1 {
    grid-area: name;
    margin: 10px;
  }
  &__modal-item2 {
    grid-area: about;
    margin: 10px;
  }
  &__modal-item3 {
    grid-area: skills;
    margin: 10px;
  }
  &__modal-item4 {
    grid-area: portfolio;
    margin: 10px;
  }
  &__modal-item5 {
    grid-area: contacts;
    margin: 10px;
  }
  &__modal-item6 {
    grid-area: close;
    margin: 10px;
    justify-self: end;
    img {
      width: 20px;
      &:hover {
        cursor: pointer;
      }
    }
  }
  &__modal-item7 {
    grid-area: lang;
    justify-self: end;
    transform: rotate(90deg);
    margin-right: -13%;
    height: 70px;
  }
  @media (max-width: 540px) {
    width: 95%;
  }
  @media (max-width: 375px) {
    width: 95%;
  }
}

.hide {
  display: none !important;
}
</style>

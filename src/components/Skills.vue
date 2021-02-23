<template>
  <div class="skills">
    <div class="skills__title title">Skills</div>
    <div class="skills__text">In my work I use such technologies as</div>
    <div class="skills__items">
      <div class="skills__item">
        <div class="skills__item-icon">
          <img src="@/assets/html.png" alt="img" />
        </div>
        <div class="skills__item-desc">HTML</div>
      </div>
      <div class="skills__item">
        <div class="skills__item-icon">
          <img src="@/assets/css.png" alt="img" />
        </div>
        <div class="skills__item-desc">CSS</div>
      </div>

      <div class="skills__item">
        <div class="skills__item-icon">
          <img src="@/assets/js.png" alt="img" />
        </div>
        <div class="skills__item-desc">JavaScript</div>
      </div>

      <div class="skills__item">
        <div class="skills__item-icon">
          <img src="@/assets/vue.png" alt="img" />
        </div>
        <div class="skills__item-desc">Vue.js</div>
      </div>

      <div class="skills__item">
        <div class="skills__item-icon">
          <img src="@/assets/sass.png" alt="img" />
        </div>
        <div class="skills__item-desc">Sass/Scss</div>
      </div>
      <div class="skills__item">
        <div class="skills__item-icon">
          <img src="@/assets/git.png" alt="img" />
        </div>
        <div class="skills__item-desc">Git</div>
      </div>

      <div class="skills__item">
        <div class="skills__item-icon">
          <img src="@/assets/webpack.png" alt="img" />
        </div>
        <div class="skills__item-desc">Webpack</div>
      </div>

      <div class="skills__item">
        <div class="skills__item-icon">
          <img src="@/assets/firebase.png" alt="img" />
        </div>
        <div class="skills__item-desc">Firebase</div>
      </div>
      <div class="skills__item">
        <div class="skills__item-icon">
          <img src="@/assets/figma.png" alt="img" />
        </div>
        <div class="skills__item-desc">Figma</div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.skills {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  height: 610px;
  @media (max-width: 750px) {
    margin-top: 200px;
  }
  @media (max-width: 375px) {
    margin-top: 400px;
  }
  &__title {
    text-align: center;
    @media (max-width: 750px) {
      margin-bottom: 20px;
    }
  }
  &__text {
    text-align: center;
    @media (max-width: 750px) {
      margin-bottom: 40px;
    }
  }
  &__items {
    display: flex;
    justify-content: space-evenly;
    @media (max-width: 750px) {
      margin: 0 auto;
      width: 200px;
      flex-wrap: wrap;
    }
    @media (max-width: 375px) {
      margin: 0 auto;
      width: 100px;
      flex-wrap: wrap;
    }
  }
  &__item {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    text-align: center;
    img {
      width: 60px;
    }
  }
  &__item-desc {
    margin-bottom: 40px;
  }
}
</style>

<template>
  <div class="skills">
    <div class="skills__title title">Skills</div>
    <div class="skills__text">Use such technologies as</div>
    <div class="skills__items">
      <div class="skills__item" v-for="(item, index) in srcs" :key="index">
        <div class="skills__item-icon">
          <img :src="require(`../assets/${item}.png`)" :alt="img" />
        </div>
        <div class="skills__item-desc">{{ item }}</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    srcs: [
      'Html',
      'Css',
      'JavaScript',
      'Vue',
      'Sass-Scss',
      'Git',
      'Webpack',
      'Firebase',
      'Figma',
    ],
  }),
}
</script>

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

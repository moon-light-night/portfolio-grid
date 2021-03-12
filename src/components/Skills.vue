<template>
  <div class="skills">
    <div class="skills__title"><a name="skills">Skills</a></div>
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
@import '@/profile/variables.scss';
@import '@/profile/mixins.scss';

.skills {
  display: flex;
  flex-direction: column;
  padding: 91px 0 0 0;
  @media (max-width: $phone_sz) {
    height: auto;
  }
  &__title {
    @include style_title;
    margin: 0 0 69px 0;
  }
  &__text {
    text-align: center;
    margin: 0 0 83px 0;
  }
  &__items {
    display: flex;
    justify-content: space-evenly;
    margin: 0 0 110px 0;
    @media (max-width: 750px) {
      flex-wrap: wrap;
    }
    @media (max-width: $phone_sz) {
      margin: 0 auto 110px;
      width: 100px;
      flex-wrap: wrap;
    }
  }
  &__item {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    text-align: center;
    margin: 10px;
    img {
      width: 60px;
    }
    &:hover {
      cursor: pointer;
      .skills__item-icon {
        transition: 0.3s linear;
        transform: scale(1.1);
      }
      .skills__item-desc {
        transition: 0.3s linear;
        color: rgb(190, 12, 12);
      }
    }
  }
}
</style>

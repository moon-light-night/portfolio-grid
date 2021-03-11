<template>
  <div class="about">
    <div class="about__title"><a name="about">About me</a></div>
    <div class="about__text">
      Hi, I am Ilya – Frontend-developer from Stavropol. I'm interested in
      creating websites and everything connected with it.<br /><br />
      I'm studying at courses "Web and mobile developing" in IT-Academy.<br /><br />
      Ready to implement excellent projects with wonderful people.
    </div>
  </div>
</template>

<style lang="scss" scoped>
@import '@/profile/mixins.scss';

.about {
  width: 100%;
  background-color: rgb(235, 223, 223);
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  padding: 120px 0 0 0;
  &__title {
    @include style_title;
    margin: 0 0 18px 0;
  }
  &__text {
    @include style_text;
    text-align: center;
    width: 485px;
    margin: 0 auto 107px;
    @media (max-width: 650px) {
      width: 90%;
    }
  }
}
</style>

<template>
  <div class="about">
    <div class="about__title title">About me</div>
    <div class="about__text">
      Hi, – UX/UI designer from Minsk. I'm interested in design and everything
      connected with it.<br /><br />
      I'm studying at courses "Web and mobile design interfaces" in
      IT-Academy.<br /><br />
      Ready to implement excellent projects with wonderful people.
    </div>
  </div>
</template>

<style lang="scss" scoped>
.about {
  width: 100%;
  height: 506px;
  background-color: rgba(246, 246, 246, 1);
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  &__title {
    text-align: center;
  }
  &__text {
    text-align: center;
    width: 485px;
    margin: 0 auto;
    font-size: 18px;
    @media (max-width: 650px) {
      width: 90%;
    }
  }
}
</style>

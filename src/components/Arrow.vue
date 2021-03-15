<template>
  <div class="arrow">
    <a href="#home"
      ><svg class="arrow-item">
        <use xlink:href="#arrow"></use></svg
    ></a>
  </div>
</template>

<style lang="scss">
.arrow {
  position: fixed;
  left: 15px;
  bottom: 15px;
}
.arrow-item {
  width: 48px;
  height: 48px;
  opacity: 0.2;
  transition: 0.3s linear;
  border-radius: 50%;
  &:hover {
    cursor: pointer;
    opacity: 1;
    background-color: rgb(190, 12, 12);
  }
}
#arrow {
  &:hover {
    cursor: pointer;
  }
}
</style>

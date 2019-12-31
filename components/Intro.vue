<template>
  <div class="intro">
    <div class="intro__header">
      <div class="intro__logo">
        logo
      </div>
      <div class="intro__hamburger">
        hamburger
      </div>
    </div>

    <div class="intro__content">
      <div class="intro__text">
        <div class="intro__headline">
          Headline
        </div>

        <div class="intro__description">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aut laborum nam nemo perferendis quasi quo quod rem
          sit tempore vero.
        </div>

        <div class="intro__button">
          Button
        </div>
      </div>

      <div class="intro__play">
        play button
      </div>
    </div>

    <div class="intro__footer">
      <div class="intro__footer-headline">
        Lorem ipsum dolor sit.
      </div>

      <div class="intro__clients">
        <div>microsoft</div>
        <div>boosted</div>
        <div>hallmark</div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "Intro"
  }
</script>

<style lang="scss" scoped>
  .intro {
    position: relative;
    height: 100vh;
    width: 100vw;
    display: flex;
    flex-direction: column;
    flex: 1;

    &__header {
      height: 80px;
      width: 100%;
      background-color: yellow;
      color: #000;
      display: flex;
      align-items: flex-end;
      justify-content: space-between;
    }

    &__logo {
      margin-left: 20px;
    }

    &__hamburger {
      margin-right: 20px;
    }

    &__content {
      width: 100%;
      background-color: red;
      display: flex;
      flex: 1;
      justify-content: space-between;
      align-items: center;
    }

    &__footer {
      height: 96px;
      width: 100%;
      background-color: blue;
      display: flex;
      justify-content: space-between;
    }

    &__clients {
      display: flex;
    }
  }
</style>

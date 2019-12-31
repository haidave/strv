<template>
  <div class="intro">
    <div class="intro__header">
      <a href="#" class="intro__logo">
        <svg xmlns="http://www.w3.org/2000/svg" height="32" width="64">
          <path
            d="M60 31.2h-6L50.2.8h4.1L57 25.6 59.7.8h4.1zm-17.4 0L39 18.6h-1.6v12.6h-4.2V.8h7.3c1.6 0 2.9.5 4 1.5 1 1 1.6 2.6 1.6 4.9v4.7c0 1.5-.3 2.8-.8 3.8-.6 1-1.3 1.7-2.2 2.1L47 31.3h-4.4zm-.8-23.5c0-1.1-.2-1.9-.6-2.4s-1-.7-1.8-.7h-2.1v10h2.1c.8 0 1.4-.2 1.8-.7s.6-1.2.6-2.4zm-17-2.9v26.4h-4.1V4.8h-4.3v-4h12.8v4zM11 30c-1.2 1-2.7 1.5-4.6 1.5S3 31 1.8 29.9C.6 28.9 0 27.2 0 25.1v-4.3h4.1v3.8c0 1.1.2 1.9.7 2.4s1 .7 1.6.7 1.1-.2 1.6-.7.7-1.2.7-2.4v-2.5c0-.6-.2-1.1-.6-1.7-.4-.5-1-1.1-1.6-1.7s-1.3-1.2-2.1-1.8-1.5-1.3-2.1-2-1.2-1.5-1.6-2.3-.6-1.7-.6-2.7V6.4c0-1.1.2-2.1.5-2.9S1.4 2 2 1.5 3.3.6 4 .4C4.8.2 5.6 0 6.5 0S8.2.1 9 .4c.8.2 1.5.6 2 1.1.6.5 1.1 1.2 1.4 2s.5 1.8.5 2.9v4.4H8.8V6.9c0-1.1-.2-1.9-.7-2.4s-1-.7-1.6-.7-1.1.2-1.6.7-.7 1.2-.7 2.4v2.2c0 .8.2 1.5.6 2.1s1 1.2 1.6 1.8 1.3 1.1 2.1 1.7 1.5 1.1 2.1 1.8c.6.6 1.2 1.3 1.6 2s.6 1.6.6 2.6v3.8c0 2.5-.6 4.1-1.8 5.1z"
            fill="#ef0d33" fill-rule="evenodd"/>
        </svg>
      </a>

      <div class="intro__hamburger">
        <span class="hamburger__line hamburger__line-1"></span>
        <span class="hamburger__line hamburger__line-2"></span>
        <span class="hamburger__line hamburger__line-3"></span>
      </div>
    </div>

    <div class="intro__bg">
      <video muted autoplay loop>
        <source src="~assets/videos/bg.mp4" type="video/mp4">
      </video>
    </div>

    <div class="intro__content">
      <div class="intro__text">
        <div class="intro__headline">
          Next level<br/>
          Design &<br class="hidden"/>
          Technology
        </div>

        <div class="intro__divider"></div>

        <div class="intro__description">
          You have the vision for a stunning digital experience. We’re<br/>
          the software design and engineering team that can bring it to life.
        </div>

        <div class="intro__button">
          <span class="intro__button-text">
            Let's Get Started
          </span>
        </div>
      </div>

      <div class="intro__play">
        <div class="intro__play-icon"></div>
      </div>
    </div>

    <div class="intro__footer">
      <div class="intro__footer-headline">
        We've built solutions for...
      </div>

      <div class="intro__clients">
        <img class="intro__clients--microsoft" src="~assets/logos/microsoft.png" alt="Microsoft">
        <img class="intro__clients--boosted" src="~assets/logos/boosted.png" alt="Boosted">
        <img class="intro__clients--hallmark" src="~assets/logos/hallmark.png" alt="Hallmark">
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
  .hidden {
    display: none;
  }
  .intro {
    position: relative;
    height: 100vh;
    width: 100vw;
    display: flex;
    flex-direction: column;
    flex: 1;

    &__bg {
      position: absolute;
      top: 0;
      left: 0;
      height: 100%;
      width: 100%;
      overflow: hidden;
      z-index: -1;
    }

    &__header {
      position: relative;
      height: 80px;
      width: 100%;
      display: flex;
      align-items: flex-end;
      justify-content: space-between;
    }

    &__logo {
      position: absolute;
      left: 49px;
      width: 64px;
      height: 32px;
    }

    &__hamburger {
      position: absolute;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      right: 43px;
      width: 64px;
      height: 30px;
      cursor: pointer;
    }

    .hamburger__line {
      display: block;
      width: 32px;
      height: 3px;
      background: #ffffff;

      &-2,
      &-3 {
        margin-top: 5px;
      }
    }

    &__content {
      width: 100%;
      display: flex;
      flex: 1;
      justify-content: space-between;
      align-items: center;
    }

    &__text {
      flex: 1;
      padding-left: 130px;
    }

    &__headline {
      font-family: 'Trump Gothic East', sans-serif;
      font-size: 5.5rem;
      line-height: 1;
      text-transform: uppercase;
    }

    &__divider {
      width: 40px;
      height: 4px;
      margin: 30px 0;
      background-color: #ef0d33;
    }

    &__description {
      font-family: 'Maison Neue', sans-serif;
      font-size: 1.125rem;
      font-weight: 300;
      line-height: 1.4;
    }

    &__button {
      width: 240px;
      margin-top: 25px;
      background-color: #ef0d33;
      border: 2px solid transparent;
      border-radius: 2px;
      padding: 24px 0 20px;
      text-align: center;

      &-text {
        font-family: 'Maison Neue', sans-serif;
        font-size: 1rem;
        font-weight: 600;
        letter-spacing: 2px;
        text-transform: uppercase;
      }
    }

    &__play {
      display: flex;
      justify-content: center;
      flex: 1;
      margin-top: -60px;
      padding-right: 130px;

      &-icon {
        width: 120px;
        height: 120px;
        border: 4px solid #ef0d33;
        border-radius: 50%;
      }
    }

    &__footer {
      position: relative;
      height: 96px;
      width: 100%;
      /*border-top: 1px solid #dededf; //opacity: 0.2*/
      display: flex;
      justify-content: space-between;
      align-items: center;

      &::before {
        content: '';
        position: absolute;
        left: 130px;
        right: 130px;
        top: 0;
        height: 1px;
        background-color: #dededf;
        opacity: 0.2;
      }

      &-headline {
        font-family: 'Maison Neue', sans-serif;
        font-size: 0.9375rem;
        font-weight: 500;
        letter-spacing: .09375rem;
        line-height: 1.5rem;
        text-transform: uppercase;
        padding-left: 130px;
      }
    }

    &__clients {
      max-width: 550px;
      padding-left: 30px;
      padding-right: 130px;
      display: flex;
      flex: 1 0 auto;
      align-items: center;
      justify-content: space-between;

      &--microsoft {
        height: 24px;
        width: 114px;
      }

      &--boosted {
        height: 32px;
        width: 132px;
      }

      &--hallmark {
        height: 27px;
        width: 103px;
      }
    }
  }
</style>

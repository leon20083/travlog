<template>
  <!-- Начало: Данный блок удалять нельзя -->
  <div class="maketforfigma">
    <a href="https://t.me/s/FigmaToHTML" target="_blank">
      <img src="./assets/img/logo.png" />
    </a>
    <div>
      <p>
        Данная верстка, была реализована пользователем в рамках обучающего
        телеграм канал
        <a href="https://t.me/s/FigmaToHTML" target="_blank"
          >FIGMA | Макеты для верстки</a
        >
      </p>
      <p>
        При помощи
        <a href="https://t.me/HtmlCodeForMoney_bot?from_git" target="_blank"
          >Telegram-бота</a
        >
        пользователь получил оплату за верстку этого макета.
      </p>
    </div>
  </div>
  <!-- Конец -->
  <div class="top-gradient"></div>

  <Header />
  <TravelTop />
  <OwlCarousel />
  <TopDestination />
  <TravelPoint />
  <KeyFeatures />
</template>

<script>
import Header from "./components/Header.vue";
import TravelTop from "./components/TravelTop.vue";
import OwlCarousel from "./components/OwlCarousel.vue";
import TopDestination from "./components/TopDestination.vue";
import TravelPoint from "./components/TravelPoint.vue";
import KeyFeatures from "./components/KeyFeatures.vue";
export default {
  name: "App",
  components: {
    Header,
    TravelTop,
    OwlCarousel,
    TopDestination,
    TravelPoint,
    KeyFeatures,
  },
};
</script>

<style lang="sass">
.top-gradient
  position: absolute
  top: 0
  left: 0
  height: 300px
  width: 300px
  border-radius: 500px
  opacity: 0.5
  background: #FF5722
  filter: blur(250px)
.right-gradient
  position: absolute
  bottom: 0
  right: 0
  height: 300px
  width: 300px
  border-radius: 500px
  opacity: 0.5
  background: #FF5722
  filter: blur(250px)
</style>

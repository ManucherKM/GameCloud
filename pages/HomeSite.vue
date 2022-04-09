<template>
  <div class="home-wrapper">
    <NavBarSite class="menu" />
    <div class="container">
      <div class="home-wrapper__slide">
        <img src="../assets/img/Home/Slide.png" alt="Photo" class="home-wrapper__item" />
        <div class="text-slider">
          <div class="app-block-title">
            <hr class="home-line-one" />
            <p class="app__subtitle">Сервис облачного гейминга</p>
            <h1 class="app__title">Преврати свое устройство в игровое</h1>
          </div>

          <div class="app__btn">
            <nuxt-link to="/HomeSite">
              <ButtonSite :text="textBtn" />
            </nuxt-link>
            <hr class="home-line-one" />
          </div>
        </div>
      </div>
      <div class="How-it-works">
        <div class="container">
          <div class="block-left">
            <img src="../assets/img/Home/img-block-2.png" alt="Photo" class="block-left__img" />
          </div>
          <div class="block-right">
            <SubtitleHome :text="textSubtitleOne" />
            <p class="block-right-title">Как это работает</p>
            <p class="block-right-subtitle">
              Наши сервера запускают игру, и передают
              вам картинку, которой вы можете управлять
              в реальном времени!
            </p>
            <hr class="block-right-line-two" />
            <p class="block-right-subtitle">
              Приложение запустится на ПК с процессором
              от 1.5 GHz , от 1 Gb RAM и доступом в интернет
              от 15 мбит/с
              на всех операционых системах
              Windows 7, 8, 10 MacOS и Linux .
            </p>
            <Textunderline :text="textUnderlineOne" />
          </div>
        </div>
      </div>
      <div class="quick-start">
        <div class="container">
          <div class="block-title">
            <SubtitleHome class="title-one" :text="textSubtitleTwo" />
            <p class="block-right-title title-two">Начни играть</p>
          </div>

          <div class="quick-start__block-body">
            <div class="block-body__iteme">
              <img
                src="../assets/img/Home/block-2/Mail Contact.svg"
                alt="Photo"
                class="quick-start-img"
              />
              <p class="quick-start__item-text">Создайте аккаунт</p>
            </div>
            <hr class="quick-start-line" />
            <div class="block-body__iteme">
              <img
                src="../assets/img/Home/block-2/Download from the Cloud.svg"
                alt="Photo"
                class="quick-start-img"
              />
              <p class="quick-start__item-text">Cкачайте модуль</p>
            </div>
            <hr class="quick-start-line" />
            <div class="block-body__iteme">
              <img src="../assets/img/Home/block-2/Library.svg" alt="Photo" class="quick-start-img" />
              <p class="quick-start__item-text">Выберите тариф</p>
            </div>
            <hr class="quick-start-line" />
            <div class="block-body__iteme">
              <img
                src="../assets/img/Home/block-2/Apple Arcade.svg"
                alt="Photo"
                class="quick-start-img"
              />
              <p class="quick-start__item-text">Начни играть</p>
            </div>
          </div>
          <Textunderline class="text-center" :text="textUnderlineTwo" />
        </div>
      </div>
      <div class="avble-sub">
        <div class="block-title">
          <SubtitleHome class="title-one" :text="textSubtitleThree" />
          <p class="block-right-title title-two">Доступные подписки</p>
        </div>
        <div class="wrapper-cards">
          <CardSub :sum="sumOne" :mas="list" />
          <CardSub :sum="sumTwo" :mas="list" />
          <CardSub :sum="sumThree" :mas="list" />
        </div>
        <hr class="avble-sub__line" />
      </div>
      <div class="cros-platform">
        <div class="block-right">
          <SubtitleHome :text="textSubtitleFour" />
          <p class="block-right-title">Запускайте на любых устройствах</p>
          <p class="block-right-subtitle">
            Наш модуль доступен на все популярные ОС
            и работает на всех компьютерах.
          </p>
          <Textunderline :text="textUnderlineThree" />
        </div>
        <div class="block-left"></div>
      </div>
      <div class="wrapper-block-six">
        <div class="wrapper-block-six__title">
          <SubtitleHome :text="textSubtitleFive" />
          <p class="block-right-title">Карта локаций</p>
          <img src="../assets/img/Home/block-6/img.png" alt="Photo" class="wrapper-block-six__img" />
        </div>
      </div>
      <div class="footer">
        <div class="container">
          <div class="block-right">
            <nuxt-link to="/HomeSite">
              <LogoAndText class="del" />
            </nuxt-link>

            <a href="#" class="text">2022. All rights reserved.</a>
            <a href="#" class="text disable">Design by desart</a>
          </div>
          <div class="block-left">
            <a href="#" class="text-right">Политика конфиденциальности</a>
            <a href="#" class="text-right">Файлы Coocie</a>
            <div class="wrapper-contact__name">
              <div class="social-parent">
                <a href="https://vk.com/" target="_blank">
                  <img src="../assets/img/pageContact/VK.svg" alt="Photo" class="social" />
                </a>
              </div>
              <div class="social-parent">
                <a href="https://discord.com/" target="_blank">
                  <img src="../assets/img/pageContact/Discord.svg" alt="Photo" class="social" />
                </a>
              </div>
              <div class="social-parent">
                <a href="https://www.youtube.com/" target="_blank">
                  <img src="../assets/img/pageContact/YouTube.svg" alt="Photo" class="social" />
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import NavBarSite from "../components/NavBarSite.vue";
import SubtitleHome from "../components/SubtitleHome.vue";
import Textunderline from "../components/textunderline.vue";
import CardSub from "../components/CardSub.vue";
import LogoAndText from "../components/LogoAndText.vue";
export default {
  data() {
    return {
      textBtn: "UPGRADE",
      textSubtitleOne: "Облачный гейминг",
      textSubtitleTwo: "Быстрый старт",
      textSubtitleThree: "Гибкие тарифы",
      textSubtitleFour: "Играть можно в браузере",
      textSubtitleFive: "Игровые сервера на карте",
      textUnderlineOne: "Загрузить",
      textUnderlineTwo: "Начать",
      textUnderlineThree: "Открыть в браузере",
      sumOne: "45 р.  -  час",
      sumTwo: "2999 р.  -  месяц",
      sumThree: "1500 р.  -  месяц",
      list: ["Каталог игр", "Виртуальный ПК", "Игровая сессия 10 часов/день"]
    }
  },
  components: { NavBarSite, SubtitleHome, Textunderline, CardSub, LogoAndText }
}
</script>

<style>
</style>
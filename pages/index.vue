<template>
  <div class="app">
    <div class="app-bg">
      <div class="app-shadow"></div>
      <div ref="opacOne" class="app__slider">
        <SlideHome />
      </div>
      <div ref="opacThree" class="app-block-title">
        <p class="app__subtitle">Сервис облачного гейминга</p>
        <h1 class="app__title">Преврати свое устройство в игровое</h1>
      </div>
      <nuxt-link to="/HomeSite">
        <div ref="opacTwo" class="app__btn">
          <ButtonSite :text="textBtn" />
        </div>
      </nuxt-link>
      <hr class="app__line-bottom" />
      <div ref="opacFour" class="app__block-right">
        <img src="../assets/img/page1/burger.svg" alt="Photo" class="block-right-img" />
        <hr class="app__line-right" />
      </div>
    </div>
  </div>
</template>

<script>
import SlideHome from "../components/SlideHome.vue";
import ButtonSite from "../components/ButtonSite.vue";
export default {
  name: "IndexPage",
  data() {
    return {
      textBtn: "UPGRADE"
    }
  },
  methods: {
    run() {
      console.log(123)
      setTimeout(() => {
        this.$refs.opacOne.style.opacity = "1";
        this.$refs.opacThree.style.opacity = "1";
        this.$refs.opacFour.style.opacity = "1";
      }, 4000);
      setTimeout(() => {
        this.$refs.opacThree.style.opacity = "1";
      }, 4000);
      setTimeout(() => {
        this.$refs.opacFour.style.opacity = "1";
      }, 4000);
      setTimeout(() => {
        this.$refs.opacTwo.style.opacity = "1";
      }, 4000);
    }
  },
  beforeMount() {
    this.run()
  },
  components: { SlideHome, ButtonSite }
}
</script>

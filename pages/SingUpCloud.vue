<template>
    <div class="wrapper-reg">
        <div class="wrapper-config__title">
            <nuxt-link to="/" class="link">
                <img
                    src="../assets/img/pageSingIn/arrow-back.svg"
                    alt="Photo"
                    class="arrow-back-img"
                />
            </nuxt-link>
            <nuxt-link to="/SingUpCloud" class="title">Регестрация</nuxt-link>
            <nuxt-link to="/SingInCloud" class="title disable-link">Вход</nuxt-link>
        </div>
        <div class="wrapper-reg__block">
            <InputSite :typeInput="inpOneType" :placeholderInput="inpOnePlaeceholder" />
            <InputSite :typeInput="inpTwoType" :placeholderInput="inpTwoPlaeceholder" />
        </div>
        <div class="block-button">
            <ButtonSite :text="textBtn" />
        </div>
        <div class="wrapper-reg__block-checkbox">
            <div class="wrapper-checkbox">
                <input type="checkbox" id="horns" name="horns" />
                <label for="horns"></label>
            </div>
            <div class="block-checkbox-text">
                <p
                    class="text-chkbox"
                >Я соглашаюсь со следующими установленными правилами: Политика использования файлов cookie WARPLAY.CLOUD, Пользовательское соглашение WARPLAY.CLOUD, Лицензионное соглашение MY.GAMES с конечным пользователем в отношении Игр, Лицензионное соглашение с конечным Пользователем для WARPLAY.CLOUD Игрового центра, Политика конфиденциальности портала WARPLAY.CLOUD, Политика конфиденциальности WARPLAY.CLOUD для детей</p>
            </div>
        </div>
        <div class="wrapper-line">
            <hr class="wrapper-line__line" />
            <p class="wrapper-line__text">Войти через</p>
            <hr class="wrapper-line__line" />
        </div>
        <div class="wrapper-social-media">
            <div class="wrapper-social-media__top">
                <a href="https://mail.ru/" target="_blank" class="socual-top__link">
                    <img src="../assets/img/SingUpCloud/Mail.ru.svg" alt="Photo" class="top-social" />
                </a>
                <a href="https://vk.com/" target="_blank" class="socual-top__link">
                    <img src="../assets/img/SingUpCloud/VK.svg" alt="Photo" class="top-social" />
                </a>
                <a href="https://ok.ru/" target="_blank" class="socual-top__link">
                    <img src="../assets/img/SingUpCloud/OK.svg" alt="Photo" class="top-social" />
                </a>
                <a href="https://ru-ru.facebook.com/" target="_blank" class="socual-top__link">
                    <img
                        src="../assets/img/SingUpCloud/Facebook.svg"
                        alt="Photo"
                        class="top-social"
                    />
                </a>
                <a href="https://www.google.com/" target="_blank" class="socual-top__link">
                    <img src="../assets/img/SingUpCloud/Google.svg" alt="Photo" class="top-social" />
                </a>
            </div>
            <div class="wrapper-social-media__bottom">
                <a href="https://www.twitch.tv/" target="_blank" class="socual-top__link">
                    <img
                        src="../assets/img/SingUpCloud/Twitch.svg"
                        alt="Photo"
                        class="bottom-social"
                    />
                </a>
                <a href="https://twitter.com/" target="_blank" class="socual-top__link">
                    <img
                        src="../assets/img/SingUpCloud/Twitter.svg"
                        alt="Photo"
                        class="bottom-social"
                    />
                </a>
                <a href="https://www.apple.com/ru/" target="_blank" class="socual-top__link">
                    <img
                        src="../assets/img/SingUpCloud/Apple.svg"
                        alt="Photo"
                        class="bottom-social"
                    />
                </a>
            </div>
        </div>
    </div>
</template>

<script>
import ButtonSite from '../components/ButtonSite.vue'
import InputSite from '../components/InputSite.vue'
export default {
    data() {
        return {
            inpOneType: "E-mail",
            inpOnePlaeceholder: "Почта / Телефон",
            inpTwoType: "password",
            inpTwoPlaeceholder: "Пароль",
            textBtn: "Зарегестрироваться"
        }
    },
    components: { InputSite, ButtonSite },

}
</script>

<style>
</style>
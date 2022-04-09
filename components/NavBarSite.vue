<template>
    <div class="nav-bar">
        <div class="container">
            <LogoAndText class="logo" />
            <ul class="nav-bar__list">
                <li class="nav-bar-item">
                    <nuxt-link to="/HomeSite" class="nav-bar__link">Главная</nuxt-link>
                </li>
                <li class="nav-bar-item">
                    <nuxt-link to="/AvSub" class="nav-bar__link">Сервера</nuxt-link>
                </li>
                <li class="nav-bar-item">
                    <nuxt-link to="/DowlandFile" class="nav-bar__link">Скачать</nuxt-link>
                </li>
                <li class="nav-bar-item">
                    <nuxt-link to="/" class="nav-bar__link">Открыть в браузере</nuxt-link>
                </li>
                <li class="nav-bar-item">
                    <nuxt-link to="/AvSub" class="nav-bar__link">Цены</nuxt-link>
                </li>
                <li class="nav-bar-item">
                    <nuxt-link to="/" class="nav-bar__link">Тех поддержка</nuxt-link>
                </li>
                <li class="nav-bar-item">
                    <nuxt-link to="/" class="nav-bar__link">Контакты</nuxt-link>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
import LogoAndText from "./LogoAndText.vue";
export default {
    components: { LogoAndText }
}
</script>

<style>
</style>
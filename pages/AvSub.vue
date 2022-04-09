<template>
    <div class="wrapper-page-av-sub">
        <div class="wrapper-config__title">
            <nuxt-link to="/" class="link">
                <img
                    src="../assets/img/pageSingIn/arrow-back.svg"
                    alt="Photo"
                    class="arrow-back-img"
                />
            </nuxt-link>
            <h2 class="title">Контакты</h2>
        </div>
        <div class="wrapper-av-sub-card">
            <CardSub :sum="cardSumOne" :mas="aviablCardOne" />
            <CardSub :sum="cardSumTwo" :mas="aviablCardTwo" />
            <CardSub :sum="cardSumThree" :mas="aviablCardThree" />
        </div>
    </div>
</template>

<script>
import CardSub from "../components/CardSub.vue";
export default {
    data() {
        return {
            cardSumOne: "45 р.  -  час",
            cardSumTwo: "2999 р. - месяц",
            cardSumThree: "1500 р.  -  месяц",
            aviablCardOne: ["Каталог игр", "Виртуальный ПК", "Безлимитная игровая сессия"],
            aviablCardTwo: ["Каталог игр", "Виртуальный ПК", "Игровая сессия 10 часов/день"],
            aviablCardThree: ["Каталог игр", "Виртуальный ПК", "Игровая сессия 5 часов/день"],
        }
    },
    components: { CardSub }
}
</script>

<style>
</style>
<template>
    <div class="wrapper-card-sub">
        <div class="wrapper-card-sub__container">
            <h3 class="wrapper-card-sub__title">Подписка Максимум</h3>
            <p class="wrapper-card-sub__sum">{{ sum }}</p>
            <p class="wrapper-card-available">Доступно:</p>
            <p v-for="(item, index) in mas" :key="index" class="wrapper-card-available">{{ item }}</p>
            <CardButton class="wrapper-card-sub-mb" />
        </div>
    </div>
</template>

<script>
import CardButton from "./CardButton.vue";
export default {
    props: {
        sum: {
            type: String,
            required: true
        },
        mas: {
            type: Array,
            required: true
        },
    },
    components: { CardButton }
}
</script>

<style>
</style>
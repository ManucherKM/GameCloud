<template>
    <div class="wrapper-button">
        <button class="wrapper-button__button">{{ text }}</button>
    </div>
</template>

<script>
export default {

    props: {
        text: {
            type: String,
            required: true
        }
    }

}
</script>

<style>
</style>
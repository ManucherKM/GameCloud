<template>
    <div>
        <div class="block-right-one-title">
            <hr class="one-title__line" />
            <p class="one-title__text">{{ text }}</p>
        </div>
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
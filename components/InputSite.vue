<template>
    <div class="wrapper-input">
        <input :placeholder="placeholderInput" class="wrapper-input__input" :type="typeInput" />
    </div>
</template>

<script>
export default {
    props: {
        typeInput: {
            type: String,
            required: true
        },

        placeholderInput: {
            type: String,
            required: true
        },
    }

}
</script>

<style>
</style>
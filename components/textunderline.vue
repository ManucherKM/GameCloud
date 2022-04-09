<template>
    <div>
        <nuxt-link to="/HomePage" class="dowland-text">{{ text }}</nuxt-link>
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
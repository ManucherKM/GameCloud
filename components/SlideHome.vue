<template>
    <div class="parentTwo">
        <div class="parenTwo-border">
            <LogoAndText />
            <div ref="div" class="parentTwo-br">
                <img
                    ref="sliedrImgOne"
                    key="One"
                    class="parentTwo-br pos z-one"
                    src="../assets/img/page1/game-one.png"
                    alt="Photo"
                />
                <img
                    ref="sliedrImgTwo"
                    key="Two"
                    class="parentTwo-br pos z-two"
                    src="../assets/img/page1/game-two.png"
                    alt="Photo"
                />
                <img
                    ref="sliedrImgThree"
                    key="Three"
                    class="parentTwo-br pos z-three"
                    src="../assets/img/page1/game-three.png"
                    alt="Photo"
                />
            </div>
        </div>
    </div>
</template>

<script scoped>
import LogoAndText from "./LogoAndText.vue";


export default {
    components: { LogoAndText }
}
</script>

<style>
</style>
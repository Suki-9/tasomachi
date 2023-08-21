<script setup lang="ts">
//Vue Component
import HeadBarVue from "../components/global/HeadBar.vue";

</script>


<template>
    <HeadBarVue />
    <img :class="$style.headImg" src="../assets/imgs/Head.webp" />
</template>


<style module lang="scss">
.headImg {
    margin-top: 7vh;
    width: 100Vw;
}
</style>
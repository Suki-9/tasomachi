<script setup lang="ts">
const props = defineProps<{
    textData: {
        title: string;
        texts: string[];
    }
}>();

</script>


<template>
    <div :class="$style.root">
        <h1>{{ textData.title }}</h1>
        <p v-for="text in textData.texts" v-text="text"></p>
    </div>
</template>


<style module lang="scss">
.root {
    width: min(100%, 900px);

    font-size: 120%;
    h1 {
        border-bottom: solid 1px;
    }
    p {
        margin-bottom: 2em;
    }
}
</style>
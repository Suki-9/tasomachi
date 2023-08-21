<script setup lang="ts">
//Vue Component
import TextBoxVue from "../global/TextBox.vue";

//text
import { gameDescription_ja } from "../../texts/text";
</script>


<template>
    <div :class="$style.root" id="gameDescription">
        <TextBoxVue :textData="gameDescription_ja" />
        <iframe src="https://www.youtube-nocookie.com/embed/8sLEZYuOIrE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
        <h1>
            2021年4月14日発売(PC)<br>
            2022年4月28日発売（Switch/PS4）
        </h1>
    </div>
</template>

<style module lang="scss">
.root {
    display: flex;
    flex-direction: column;
    align-items: center;

    margin: 10px 0 10px 0;

    background-color: var(--bg-color-002);
    color: var(--text-color-002);

    iframe {
        width: 80%;
        max-width: 900px;
        height: calc(900px/16*9);
    }
    h1 {
        text-align: center;
    }
}
</style>
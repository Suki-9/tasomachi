<script setup lang="ts">

</script>
    

<template>
    <div :class="$style.root">
        <p :class="$style.title">黄昏ニ眠ル街</p>
        <div :class="$style.menuBox">
            <a>ホーム</a>
            <a>ゲーム説明</a>
            <a>ニュース</a>
            <a>ギャラリー</a>
            <a>アート</a>
            <a>概要</a>
        </div>
    </div>
    <div :class="$style.links" v-show="false">
        <div :class="$style.icons">
            <i class="icon-link"></i>
            <i class="icon-twitter"></i>
            <i class="icon-youtube-play"></i>
            <i class="icon-globe"></i>
        </div>
    </div>
</template>

<style module lang="scss">
@import "../../assets/css/animation/hover.css";

.root {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;

    position: fixed;
    top: 0px;

    width: 100vw;

    height: 7vh;

    background-color: var(--bg-color-001);
    .title {
        padding: 0 5% 0 5%;

        font-size: 120%;
    }
    .menuBox {
        display: flex;
        justify-content: space-around;

        width: 60%;
        a {
            display: flex;
            align-items: center;
            justify-content: center;

            height: 7vh;
            width: calc(100%/7);

            padding: 0 2% 0 2%;
            margin: 0 2% 0 2%;

            white-space: nowrap;
            overflow: ellipsis;

            border-radius: 7px 7px 0 0 ;
        }
        a:hover {
            height: calc(7vh - 6px); 

            border-top:  solid 3px var(--bg-color-001);
            border-bottom:  solid 3px;
    
            animation-name: change-bg-color-001;
            animation-duration: 0.5s;
            animation-fill-mode: forwards;
        }
    }
}
.links {
    position: fixed;
    top: 7vh;
    right: 0px;

    background-color: var(--bg-color-001);

    border-radius: 0 0 0 7px;

    width: 20%;
    .icons {
        display: flex;
        justify-content: space-around;
        i {
            margin: 2%;
        }
    }
}
</style>


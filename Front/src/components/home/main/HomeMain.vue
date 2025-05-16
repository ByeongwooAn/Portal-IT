<template>
    <main class="home-main">
        <HomeTopArticle />
        <HomeMenuNav />
        <HomePostArticle />
    </main>
</template>

<script setup>
import HomeTopArticle from "./HomeTopArticle.vue";
import HomeMenuNav from "./HomeMenuNav.vue";
import HomePostArticle from "./HomePostArticle.vue";
</script>

<style scoped>
.home-main {
    width: 1285px;
    margin: 0 auto;
}
</style>

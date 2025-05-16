<template>
    <article id="top-area">
        <HomeNewsList />
        <div id="side-area">
            <HomeLoginBox />
            <HomeWeatherBox />
        </div>
    </article>
</template>

<script setup>
import HomeNewsList from "./HomeNewsList.vue";
import HomeLoginBox from "./HomeLoginBox.vue";
import HomeWeatherBox from "./HomeWeatherBox.vue";
</script>

<style scoped>
#top-area {
    display: flex;
}

#side-area {
    margin-left: 5px;
}
</style>

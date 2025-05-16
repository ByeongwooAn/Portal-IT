<template>
    <header class="home-header">
        <Logo />
        <SearchBar />
    </header>
</template>

<script setup>
import Logo from "@/components/common/Logo.vue";
import SearchBar from "@/components/home/main/SearchBar.vue";
</script>

<style scoped>
.home-header {
    width: 1280px;
    margin: 0 auto;
    padding-bottom: 41px;
    justify-items: center;
}
</style>

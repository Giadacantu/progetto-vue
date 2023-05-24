<script setup>
defineProps({
    title: String,
    abstract: String,
    imageUrl: String,
})
</script>

<template>
    <div class="section">
        <div class="image">
            <img :src="imageUrl" width="300" height="200" />
        </div>
        <div class="video-text">
            <h1>{{ title }}</h1>
            <p class="description">{{ abstract }}</p>
        </div>
    </div>
</template>

<style scoped>
img {
    display: block;
}
</style>

<script setup>

defineProps({
    title: String,
    subtitle: String,
})

</script>

<template>
    <h1 class="title">{{ title }}</h1>
    <p class="subtitle">{{ subtitle }}</p>
</template>

<style scoped>
.subtitle {
    color: #888;
}

.title {
    will-change: filter;
    transition: filter 300ms;
    filter: drop-shadow(0 0 1em #ffffff);
}
</style>

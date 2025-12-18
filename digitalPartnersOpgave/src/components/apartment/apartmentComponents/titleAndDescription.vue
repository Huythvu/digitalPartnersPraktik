<script setup>
    import { boliger } from "../../../data/data";
</script>

<template>
    <div class="titleAndDesc">
        <h1>{{ boliger[0].title }}</h1>
        <p>
            {{ boliger[0].desc }}
        </p>
    </div>
    </template>

<style scoped>
.titleAndDesc {
    display: flex;
    flex-direction: column;
    gap: 1rem;
}
</style>
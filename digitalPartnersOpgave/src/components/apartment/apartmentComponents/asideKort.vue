<script setup>
import { boliger } from "../../../data/data";
</script>

<template>
   <div class="map" v-html="boliger[0].adresse.iframe"></div>
</template>

<style scoped>
.map{
    border-radius: 10px;
    box-shadow: 4px 4px 4px rgba(0, 0, 0, 0.25);
    overflow: hidden;
}
</style>
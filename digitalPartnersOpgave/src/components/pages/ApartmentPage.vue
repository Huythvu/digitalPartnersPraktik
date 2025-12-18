<script setup>
import ImgSlider from '../apartment/ApartmentComponents/imgSlider.vue';
import introInfo from '../apartment/ApartmentComponents/introInfo.vue';
import titleAndDescription from '../apartment/ApartmentComponents/titleAndDescription.vue';
import omBolig from '../apartment/ApartmentComponents/omBolig.vue';
import omUdlejning from '../apartment/apartmentComponents/omUdlejning.vue';
import asideOmUdlejeren from '../apartment/ApartmentComponents/asideOmUdlejeren.vue';
import asideAgent from '../apartment/ApartmentComponents/asideAgent.vue';
import asideKort from '../apartment/ApartmentComponents/asideKort.vue';


</script>

<template>
    <ImgSlider />
    <main>
        <introInfo />
        <titleAndDescription />
        <omBolig />
        <omUdlejning />
        <asideOmUdlejeren />
        <asideAgent />
        <asideKort />
    </main>
</template>

<style scoped>
    main{
        margin: 4rem;
    }
</style>
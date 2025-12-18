<script setup>
import ImgSlider from '../apartment/ApartmentComponents/imgSlider.vue';
import introInfo from '../apartment/ApartmentComponents/introInfo.vue';
import titleAndDescription from '../apartment/ApartmentComponents/titleAndDescription.vue';
import omBolig from '../apartment/ApartmentComponents/omBolig.vue';
import omUdlejning from '../apartment/apartmentComponents/omUdlejning.vue';
import andreBoligerCard from '../apartment/ApartmentComponents/andreBoligerCard.vue';
import asideOmUdlejeren from '../apartment/ApartmentComponents/asideOmUdlejeren.vue';
import asideAgent from '../apartment/ApartmentComponents/asideAgent.vue';
import asideKort from '../apartment/ApartmentComponents/asideKort.vue';


</script>

<template>
    <div class="imgSlider">
        <ImgSlider />
    </div>
    <div class="container">
        <main>
            <section>
                <introInfo />
            </section>
            <section>
                <titleAndDescription />
            </section>
            <section>
                <omBolig />
            </section>
            <section>
                <omUdlejning />
            </section>
            <section>
                <andreBoligerCard />
            </section>
        </main>
        <aside>
            <asideAgent />
            <asideOmUdlejeren />
            <asideKort />
        </aside>
    </div>
</template>

<style scoped>
.imgSlider {
    margin-bottom: 2rem;
}

.container {
    display: flex;
    gap: 4rem;

    margin-bottom: 4rem;
    margin-inline: auto;
    padding-inline: 64px;
    max-width: 1620px;
}

section {
    margin-bottom: 4rem;
}

aside {
    position: sticky;
    top: 32px;
    height: fit-content;
    display: flex;
    flex-direction: column;
    gap: 2rem;
}
</style>
<script setup>
    import { boliger } from "../../../data/data";
</script>

<template>
    <div class="detaljerOmUdlejning">
        <h2>Detaljer om Udlejning</h2>
        <div class="lists">
            <ul>
        <li>Husleje pr. måned: {{ boliger[0].detaljerOmUdlejning.huslejePrMaaned }}</li>
        <li>Aconto forbrug: {{ boliger[0].detaljerOmUdlejning.acontoForbrug }}</li>
        <li>Depositum: {{ boliger[0].detaljerOmUdlejning.depositum }}</li>
        <li>Forudbetalt leje: {{ boliger[0].detaljerOmUdlejning.forudbetaltLeje }}</li>
    </ul>
    <ul>
        <li>Lejeperiode: {{ boliger[0].detaljerOmUdlejning.lejeperiode }}</li>
        <li>Indflytningsdato: {{ boliger[0].detaljerOmUdlejning.indflytningsdato }}</li>
        <li>Oprettelsesdato: {{ boliger[0].detaljerOmUdlejning.oprettelsesdato }}</li>
    </ul>
</div>
</div>
</template>

<style scoped>
    .detaljerOmUdlejning {
        display: flex;
        flex-direction: column;
        gap: 1rem;
    }
    .lists {
        display: flex;
        gap: 4rem;
    }
</style>
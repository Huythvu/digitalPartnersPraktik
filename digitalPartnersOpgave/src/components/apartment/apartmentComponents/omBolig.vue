<script setup>
    import { boliger } from "../../../data/data";
</script>

<template>
    <div class="detaljerOmBolig">
        <h2>Detaljer om bolig</h2>
        <div class="lists">
            <ul>
        <li>Boligtype: {{ boliger[0].detaljerOmBolig.boligtype }}</li>
        <li>Boligareal: {{ boliger[0].detaljerOmBolig.boligarealM2 }}</li>
        <li>Antal Værelser: {{ boliger[0].detaljerOmBolig.antalVaerelser }}</li>
        <li>Etage: {{ boliger[0].detaljerOmBolig.etage }}</li>
        <li>Energimærke: {{ boliger[0].detaljerOmBolig.energimaerke }}</li>
    </ul>
    <ul>
        <li>Altan / Terrasse: {{ boliger[0].detaljerOmBolig.altanTerrasse }}</li>
        <li>Elevator: {{ boliger[0].detaljerOmBolig.elevator }}</li>
        <li>Parkering: {{ boliger[0].detaljerOmBolig.parkering }}</li>
        <li>Vaskemaskine: {{ boliger[0].detaljerOmBolig.vaskemaskine }}</li>
        <li>Husdyr tilladt: {{ boliger[0].detaljerOmBolig.husdyrTilladt }}</li>
    </ul>
</div>
</div>
</template>

<style scoped>
    .detaljerOmBolig {
        display: flex;
        flex-direction: column;
        gap: 1rem;
    }
    .lists {
        display: flex;
        gap: 4rem;
    }
</style>
<script setup>
    import { boliger } from "../../../data/data";
</script>

<template>
    <div class="detaljerOmBolig">
        <h2>Detaljer om bolig</h2>
        <div class="lists">
    <ul>
        <li>
            <span>Boligtype:</span>
            <span>{{ boliger[0].detaljerOmBolig.boligtype }}</span>
        </li>

        <li>
            <span>Boligareal:</span>
            <span>{{ boliger[0].detaljerOmBolig.boligarealM2 }}</span>
        </li>

        <li>
            <span>Antal Værelser:</span>
            <span>{{ boliger[0].detaljerOmBolig.antalVaerelser }}</span>
        </li>
        <li>
            <span>Etage:</span>
            <span>{{ boliger[0].detaljerOmBolig.etage }}</span>
        </li>
        <li>
            <span>Energimærke:</span>
            <span>{{ boliger[0].detaljerOmBolig.energimaerke }}</span>
        </li>
    </ul>
    <ul>
        <li>
            <span>Altan / Terrasse:</span>
            <span>{{ boliger[0].detaljerOmBolig.altanTerrasse }}</span>
        </li>
        <li>
            <span>Elevator:</span>
            <span>{{ boliger[0].detaljerOmBolig.elevator }}</span>
        </li>
        <li>
            <span>Parkering:</span>
            <span>{{ boliger[0].detaljerOmBolig.parkering }}</span>
        </li>
        <li>
            <span>Vaskemaskine:</span>
            <span>{{ boliger[0].detaljerOmBolig.vaskemaskine }}</span>
        </li>
        <li>
            <span>Husdyr tilladt:</span>
            <span>{{ boliger[0].detaljerOmBolig.husdyrTilladt }}</span>
        </li>
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
    ul li {
        display: flex;
        justify-content: space-between;
        gap: 4rem;
    }
    ul li span:first-child {
        font-weight: var(--bold);
    }
</style>
<script setup>
    import { boliger } from "../../../data/data";
</script>

<template>
    <div class="detaljerOmUdlejning">
        <h2>Detaljer om Udlejning</h2>
        <div class="lists">
            <ul>
        <li>
            <span>Husleje pr. måned:</span>
            <span>{{ boliger[0].detaljerOmUdlejning.huslejePrMaaned }}</span>
        </li>
        <li>
            <span>Aconto forbrug:</span>
            <span>{{ boliger[0].detaljerOmUdlejning.acontoForbrug }}</span>
        </li>
        <li>
            <span>Depositum:</span>
            <span>{{ boliger[0].detaljerOmUdlejning.depositum }}</span>
        </li>
        <li>
            <span>Forudbetalt leje:</span>
            <span>{{ boliger[0].detaljerOmUdlejning.forudbetaltLeje }}</span>
        </li>
    </ul>
    <ul>
        <li>
            <span>Lejeperiode:</span>
            <span>{{ boliger[0].detaljerOmUdlejning.lejeperiode }}</span>
        </li>
        <li>
            <span>Indflytningsdato:</span>
            <span>{{ boliger[0].detaljerOmUdlejning.indflytningsdato }}</span>
        </li>
        <li>
            <span>Oprettelsesdato:</span>
            <span>{{ boliger[0].detaljerOmUdlejning.oprettelsesdato }}</span>
        </li>
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

    ul li {
        display: flex;
        justify-content: space-between;
        gap: 4rem;
    }
    ul li span:first-child {
        font-weight: var(--bold);
    }
</style>
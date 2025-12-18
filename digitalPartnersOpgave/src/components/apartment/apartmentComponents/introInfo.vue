<script setup>
import { boliger } from "../../../data/data";
import { ref } from "vue";

// Simple save knap funktionalitet
// Toggler  saved mellem true og false
const saved = ref(false);
const toggleSave = () => {
    saved.value = !saved.value;
};

</script>

<template>
    <div class="introInfo">
        <div class="priceInfo">
            <h2>7.700 kr./md</h2>
            <!-- Der toggler ved click og tilføjer/fjener classen gemt -->
            <button :class="{ gemt: saved }" @click="toggleSave">
                <!-- Ternary operator, fungerer ligesom if else -->
                <span class="material-icons-outlined">{{ saved ? 'favorite' : 'favorite_border' }}</span>
                <p>{{ saved ? 'Glem' : 'Gem' }}</p>
            </button>
        </div>
        <p>Dalgasgade, 9000 Aalborg</p>
        <div class="tags">
            <p>Lejlighed</p>
            <p>80 m²</p>
            <p>3 Værelser</p>
            <p>Energimærke: D</p>
        </div>
    </div>

</template>

<style scoped>
.introInfo {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
}

.priceInfo {
    display: flex;
    justify-content: space-between;
    align-items: end;
}

.tags {
    display: flex;
    gap: 0.5rem;
}

.tags p {
    background-color: var(--lightGolden);
    padding: 4px 8px;
    border-radius: 10px;
    font-size: var(--tags);
    font-weight: var(--bold);
}

button {
    display: flex;
    align-items: center;
    gap: 8px;
    cursor: pointer;

    background: none;
    border: none;
    transition: transform 1s ease-in-out;
}
button.gemt span{
    animation: pop 1s ease-in-out;
    color: red;
}

@keyframes pop {
    0% {
        transform: scale(1);
    }
    40% {
        transform: scale(1.3);
    }
    70% {
        transform: scale(0.9);
    }
    100% {
        transform: scale(1);
    }
}
</style>
<script setup>
</script>

<template>
    <div class="boligAgent">
        <div class="info">
            <h3>Kort</h3>
            <ul>
                <span class="material-symbols-outlined">favorite</span>
                <li>Valideret af DigitalBolig</li>
                <li>8 annoncer</li>
                <li>Sidst aktiv: I dag</li>
                <li>Oprettet: 13 år siden</li>
            </ul>
        </div>
        <button>Tilmeld bolig agent</button>
    </div>
</template>

<style scoped>
.boligAgent {
    background-color: var(--lightGrey);
    border-radius: 10px;
    box-shadow: 4px 4px 4px rgba(0, 0, 0, 0.25);
    padding: 1rem;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 2rem;
    width: 310px;
}

.info {
    display: flex;
    flex-direction: column;
    gap: 1rem;
}

button {
    background-color: var(--lightGolden);
    padding: 8px 16px;
    border-radius: 10px;
    cursor: pointer;
    width: max-content;
    font-size: var(--cta);
    font-weight: var(--bold);
}
</style>
<script setup>
</script>

<template>
    <div class="boligAgent">
        <div class="info">
            <h3>Bolig Agent</h3>
            <p>Tilmeld dig og få besked, når nye boliger matcher din søgning - helt gratis.</p>
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
    align-items: center;
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
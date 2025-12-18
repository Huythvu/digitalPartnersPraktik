<script setup>
</script>

<template>
    <div class="omUdlejeren">
            <h3>Om udlejeren</h3>
            <ul>
                <li>
                    <span class="material-icons-outlined">check_circle</span>
                    <span>Valideret af DigitalBolig</span>
                </li>
                <li>
                    <span class="material-icons-outlined">article</span>
                    <span>8 annoncer</span>
                </li>
                <li>
                    <span class="material-icons-outlined">schedule</span>
                    <span>Sidst aktiv: I dag</span>
                </li>
                <li>
                    <span class="material-icons-outlined">calendar_today</span>
                    <span>Oprettet: 13 år siden</span>
                </li>
            </ul>
    </div>
</template>

<style scoped>
.omUdlejeren {
    background-color: var(--lightGrey);
    border-radius: 10px;
    box-shadow: 4px 4px 4px rgba(0, 0, 0, 0.25);
    padding: 1rem;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 1rem;
    width: 310px;
}

ul {
    list-style: none;
    display: flex;
    flex-direction: column;
    gap: 1rem;
}

li {
    display: flex;
    align-items: center;
    gap: 0.5rem;
}
</style>
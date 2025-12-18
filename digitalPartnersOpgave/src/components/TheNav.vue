<script setup>
</script>

<template>
<nav>
    <a href="">DigitalBolig</a>
    <div class="navLinks">
        <a href="">Find Bolig</a>
        <a href="">Om os</a>
        <a href="">Kontakt</a>
    </div>
</nav>
</template>

<style scoped>
    nav {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 80px;
        padding-inline: 2rem;
        background-color: var(--lightGolden);
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.4);
        font-size: 32px;
    }
    .navLinks {
        display: flex;
        gap: 4rem;
        font-size: var(--cta);
    }
</style>
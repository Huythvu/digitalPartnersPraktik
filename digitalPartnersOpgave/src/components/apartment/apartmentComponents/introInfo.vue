<script setup>
    
</script>

<template>
    <div class="introInfo">
        <div class="priceInfo">
            <h2>7.700 kr./md</h2>
            <i>
                <span class="material-symbols-outlined">favorite</span>
                <p>Gem</p>
            </i>
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
.introInfo{
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
}
.priceInfo{
    display: flex;
    justify-content: space-between;
    align-items: end;
}
.tags{
    display: flex;
    gap: 0.5rem;
}
.tags p{
    background-color: var(--lightGolden);
    padding: 4px 8px;
    border-radius: 10px;
    font-size: var(--tags);
    font-weight: var(--bold);
}
i{
    display: flex;
    align-items: center;
    gap: 8px;
    cursor: pointer;
}
</style>
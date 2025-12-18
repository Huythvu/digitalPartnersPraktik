<script setup>
</script>

<template>
    <div class="andreBoliger">
        <h2>Andre boliger</h2>
        <div class="cards">
            <div class="cardsContainer">
                <img src="https://karetmagerlunden.dk/wp-content/uploads/2024/01/leje-lejlighed-horsens-stue.jpg" alt="">
                <div class="info">
                    <div class="titleAndAdress">
                        <h3>2 værelses lejlighed i Aalborg Centrum</h3>
                        <p>Dalgasgade, 9000 Aalborg</p>
                    </div>
                    <div class="priceAndDate">
                        <p>7.700 kr./md</p>
                        <p>18.December</p>
                    </div>
                </div>
            </div>
            <div class="cardsContainer">
                <img src="https://green-house.dk/uploads/slides/lejlighed-fremvisning.jpg" alt="">
                <div class="info">
                    <div class="titleAndAdress">
                        <h3>2 værelses lejlighed i Aalborg Centrum</h3>
                        <p>Dalgasgade, 9000 Aalborg</p>
                    </div>
                    <div class="priceAndDate">
                        <p>7.500 kr./md</p>
                        <p>19.December</p>
                    </div>
                </div>
            </div>
            <div class="cardsContainer">
                <img src="https://toldbodhuse.dk/uploads/boligtyper/Lejlighed-B5-2-web.jpg" alt="">
                <div class="info">
                    <div class="titleAndAdress">
                        <h3>2 værelses lejlighed i Aalborg Centrum</h3>
                        <p>Dalgasgade, 9000 Aalborg</p>
                    </div>
                    <div class="priceAndDate">
                        <p>8.500 kr./md</p>
                        <p>14.December</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    img{
    width: 100%;
    height: 200px;
    }
.andreBoliger {
    display: flex;
    flex-direction: column;
    gap: 1rem;
}

.cards {
    display: flex;
    gap: 2rem;
}

.cardsContainer {
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 4px 4px 4px rgba(0, 0, 0, 0.25);
    max-width: 310px;
}
.info {
    padding: 1rem;
    display: flex;
    flex-direction: column;
    gap: 2rem;
    background-color: var(--lightGrey);
}
.titleAndAdress {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
}
h3 {
    font-size: var(--cta);
    font-weight: var(--bold);
}
p {
    font-size: var(--smallText);
}
.priceAndDate {
    display: flex;
    justify-content: space-between;
    align-items: end;
    font-weight: var(--bold);
}
.priceAndDate p:nth-child(1) {
    font-size: var(--cta);
    font-weight: var(--bold);
}
</style>
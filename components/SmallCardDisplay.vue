<template>
    <div>
        <div class="container" v-for="displayCard in smallCardSections" :key="displayCard.id">
            <h3 class="header"> {{ displayCard.title }}</h3>
            <div class="card-container">
                <SmallCard v-for="card in displayCard.cards" :cardSections="card" :key="card.id">
                </SmallCard>
            </div>
        </div>
    </div>
</template>

<script>
import smallCardSections from '../store/smallData';
import SmallCard from '../components/SmallCard.vue';
export default {
    data() {
        return {
            smallCardSections: smallCardSections,
        }
    },
    components: {
        SmallCard
    }

}
</script>

<style  scoped>
.container {
    padding: 2rem 0
}

.header {
    font-weight: 700;
    font-size: 1.5rem;
    margin-bottom: 2rem;
}

.card-container {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}
</style>
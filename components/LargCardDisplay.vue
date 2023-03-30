<template>
    <div>
        <div class="container" v-for="cardInfo in largCardInfo" :key="cardInfo.id">
        <h4 class="header">
            {{ cardInfo.title }}
        </h4>
        <p class="snippet" >
            {{ cardInfo.snippet }}
        </p>
        <div class="cards-container">
             <LargCard 
                v-for="card in cardInfo.cards"
                :key="card.id"
                :card="card"
            />
        </div>
    </div>
    </div>
</template>

<script>
import  largeCardSections from '../store/data';
import LargCard from '../components/LargCard.vue'

export default {
 data() {
   return {
      largCardInfo: largeCardSections
   }
 },
 components: {
    LargCard
 }
}
</script>

<style scoped>
.container {
    margin-top: 2rem;
}
    .header {
        font-weight: 700;
        font-size: 1.5rem;
    }
    .snippet {
        color: grey;
        margin-bottom: 1.5rem;
    }
    .cards-container {
        display: flex;
        justify-content: space-between;
    }
</style>
<template>
  <div>
    <div class="container">
      <Hero></Hero>
      <br> <br>
      <LargCardDisplay></LargCardDisplay>
      <br>
      <smallCardSections></smallCardSections>
    </div>
  </div>
</template>

<script>
import largeCardSections from '../components/LargCardDisplay.vue';
import smallCardSections from '../components/SmallCardDisplay.vue';
export default {
  components: {
    largeCardSections,
    smallCardSections
  },
  data() {
    return {
    }
  }
}
</script>

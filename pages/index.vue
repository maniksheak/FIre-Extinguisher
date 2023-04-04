<template>
  <div class="container">
      <Navber></Navber>
      <br> <br>
       <LargCardDisplay></LargCardDisplay> 
       <br>
        <smallCardSections></smallCardSections>
  </div>
  
</template>

 <script>
 import  largeCardSections from '../components/LargCardDisplay.vue';
  import  smallCardSections from '../components/SmallCardDisplay.vue';
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

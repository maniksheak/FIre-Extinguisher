<template>
  <div class="container">
      <Navber></Navber>
      <br> <br>
       <LargCardDisplay></LargCardDisplay>
  

     
  </div>
  
</template>

 <script>
 import  largeCardSections from '../components/LargCardDisplay.vue';

export default {
  components: {
    largeCardSections
  },
  data() {
    return {
    }
  }
}
</script>

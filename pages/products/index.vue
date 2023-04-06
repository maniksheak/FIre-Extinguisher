<template>
    <div>
      <Navber />
      <LargeCardDisplay
        v-for="cardInfo in largeCardInfo"
        :key="cardInfo.id"
        :cardsSection="cardInfo"
      />
      <SmallCardDisplay 
        v-for="cardInfo in smallCardSections"
        :key="cardInfo.id"
        :cardsSection="cardInfo"
      /> 
    </div>
  </template>
  
  <script>
  import  largeCardSections  from "@/store/data.js"
   import smallCardSections from "@/store/smallData"
  export default {
    data(){
      return {
        largeCardInfo: largeCardSections,
        smallCardSections: smallCardSections
      }
    }
  }
  </script>
  
  <style>
  </style>
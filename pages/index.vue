<template>
  <div>
    <div class="header">
      <Hero />
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
  </div>
</template>

<script>
import Hero from '../components/Hero.vue'
import LargeCardDisplay from '../components/LargeCardDisplay.vue'
import { largeCardSections, smallCardSections } from '@/assets/data.js'
export default {
  components: { Hero, LargeCardDisplay },
  
  data() {
    return {
      largeCardInfo: largeCardSections,
      smallCardSections: smallCardSections
    }
  }
}
</script>

<style>

</style>
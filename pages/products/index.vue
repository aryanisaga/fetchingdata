<template>
  <div>
    <div class="header">
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
import LargeCardDisplay from '@/components/LargeCardDisplay.vue'
import SmallCardDisplay from '@/components/SmallCardDisplay.vue'
import { largeCardSections, smallCardSections } from '@/assets/data.js'
export default {
  components: { LargeCardDisplay, SmallCardDisplay },
  
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
<template>
  <div>
    <div>
      <Product/>
      <Colleague/>
      <Benefit/>
      <SecondBenefit/>
    </div>
  </div>
</template>

<script>
import ProductSection from '~/components/organisms/ProductSection.vue'
import ColleagueSection from '~/components/organisms/ColleagueSection.vue'
import BenefitSection from '~/components/organisms/BenefitSection.vue'
import SecondBenefitSection from '~/components/organisms/SecondBenefitSection.vue'
export default {
  layout: 'HeaderFooter',
  components: {
    Product: ProductSection,
    Colleague: ColleagueSection,
    Benefit: BenefitSection,
    SecondBenefit: SecondBenefitSection
  }
}
</script>

<style lang="scss" scoped>

</style>

<template>
  <div>
    <div>
      <Product/>
      <Colleague/>
      <SecondBenefit/>
    </div>
  </div>
</template>

<script>
import ProductSection from '~/components/organisms/ProductSection.vue'
import ColleagueSection from '~/components/organisms/ColleagueSection.vue'
import SecondBenefitSection from '~/components/organisms/SecondBenefitSection.vue'
export default {
  layout: 'HeaderFooter',
  components: {
    Product: ProductSection,
    Colleague: ColleagueSection,
    SecondBenefit: SecondBenefitSection
  }
}
</script>

<style lang="scss" scoped>

</style>

<template>
  <div>
    <div>
      <Product/>
      <Colleague/>
      <SpecSection/>
      <Benefit/>
      <SecondBenefit/>
      <ModuleSection/>
      <LinuxSection/>
    </div>
  </div>
</template>

<script>
import ProductSection from '~/components/organisms/ProductSection.vue'
import ColleagueSection from '~/components/organisms/ColleagueSection.vue'
import BenefitSection from '~/components/organisms/BenefitSection.vue'
import SecondBenefitSection from '~/components/organisms/SecondBenefitSection.vue'
import SpecSection from '~/components/organisms/SpecSection.vue'
import ModuleSection from '~/components/organisms/ModuleSection.vue'
import LinuxSection from '~/components/organisms/LinuxSection.vue'

export default {
  layout: 'HeaderFooter',
  components: {
    Product: ProductSection,
    Colleague: ColleagueSection,
    Benefit: BenefitSection,
    SecondBenefit: SecondBenefitSection,
    ModuleSection: ModuleSection,
    SpecSection: SpecSection,
    LinuxSection: LinuxSection,
  }
}
</script>

<style lang="scss" scoped>

</style>

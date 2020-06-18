<template>
  <div>
    <div>
      <Product/>
      <Colleague/>
    </div>
  </div>
</template>

<script>
import ProductSection from '~/components/organisms/ProductSection.vue'
import ColleagueSection from '~/components/organisms/ColleagueSection.vue'
export default {
  layout: 'HeaderFooter',
  components: {
    Product: ProductSection,
    Colleague: ColleagueSection
  }
}
</script>

<style lang="scss" scoped>

</style>

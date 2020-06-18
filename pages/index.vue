<template>
  <div>
    <div>
      <Product/>
    </div>
  </div>
</template>

<script>
import ProductSection from '~/components/organisms/ProductSection.vue'
export default {
  layout: 'HeaderFooter',
  components: {
    Product: ProductSection
  }
}
</script>

<style lang="scss" scoped>

</style>

<script setup>
import CategoryItem from './CategoryItem.vue'
</script>

<script>
export default {
  props: {
    categories: Array,
  },
}
</script>

<template>
  <div class="categories-container">
    <CategoryItem
      v-for="category in categories"
      :key="category.id"
      :title="category.title"
      :imageUrl="category.imageUrl"
    />
  </div>
</template>

<style scoped lang="scss">
.categories-container {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
</style>

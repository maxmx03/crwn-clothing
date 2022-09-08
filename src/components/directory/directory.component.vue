<script setup lang="ts">
import CategoryItemComponent from '../category-item/category-item.component.vue'
</script>

<script lang="ts">
interface Category {
  id: number
  title: string
  imageUrl: string
}

export default {
  props: {
    categories: Array<Category>,
  },
}
</script>

<template>
  <div class="categories-container">
    <CategoryItemComponent
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

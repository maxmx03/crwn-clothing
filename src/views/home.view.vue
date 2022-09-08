<script setup lang="ts">
import DirectoryComponent from '../components/directory/directory.component.vue'
import { categories } from '../utils'
</script>

<script lang="ts">
export default {
  data() {
    return {
      categories,
    }
  },
}
</script>

<template>
  <DirectoryComponent :categories="categories" />
</template>

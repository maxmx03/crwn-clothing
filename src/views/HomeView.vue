<script setup>
import Directory from '../components/Directory.vue'
import categories from '../data/categories'
</script>

<template>
  <Directory :categories="categories" />
</template>

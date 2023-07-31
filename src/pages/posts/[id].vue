<script setup>
import { useRoute } from "vue-router/auto";
const route = useRoute();
</script>
<template>
  <div>post {{ route.params.id }}</div>
</template>
<style scoped>
</style>
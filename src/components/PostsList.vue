<script setup lang="ts">
interface Props {
  post: object;
}

const props = defineProps<Props>();
</script>
<template>
  <div>
    <router-link :to="{ name: '/posts/[id]', params: { id: post.id } }">
      {{ post.title }}
    </router-link>
  </div>
</template>
<style scoped>
</style>
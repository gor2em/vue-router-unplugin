<script setup lang="ts">
import PostsList from "../../components/PostsList.vue";
import posts from "../../data/posts.json";
</script>
<template>
  <div>
    posts

    <PostsList v-for="post in posts" :key="post.id" :post="post" />
  </div>
</template>
<style scoped>
</style>
<script setup lang="ts">
import menus from "./data/menu";
</script>
<template>
  <div class="container">
    <nav>
      <ul>
        <li v-for="(menu, index) in menus" :key="index">
          <router-link :to="menu.link">{{ menu.name }}</router-link>
        </li>
      </ul>
    </nav>

    <router-link to="/notfound">go not found page</router-link>

    <main>
      <router-view></router-view>
    </main>
  </div>
</template>
<style scoped>
</style>
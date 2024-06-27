<script setup>
import { ref } from "vue";
import Header from "./components/Header.vue";
import MenueBar from "./components/MenueBar.vue";

const showMenuBar = ref(false);
</script>

<template>
  <div class="max-w-[1600px] mx-auto h-full">
    <Header @on-menu-click="showMenuBar = !showMenuBar" />
    <MenueBar :show-menu-bar="showMenuBar" />
  </div>
</template>

<style scoped></style>

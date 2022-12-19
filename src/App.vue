
<script setup lang="ts">
import HeaderVue from './components/Header.vue';
import PlayerVue from './components/Player.vue';
import MainVue from './components/Main.vue';
</script>

<template>
  <header>
    <HeaderVue></HeaderVue>
  </header>
  <main>
    <MainVue></MainVue>
  </main>
  <aside><PlayerVue></PlayerVue></aside>
</template>

<style scoped>
template{
  display: grid;
  background-color: red;
}
</style>

<script setup lang="ts">
import HeaderVue from './components/Header.vue';
import PlayerVue from './components/Player.vue';

</script>

<template>

  <main>
    <PlayerVue></PlayerVue>
    <HeaderVue></HeaderVue>

  </main>
</template>

<style scoped>
template{
  display: grid;
  background-color: red;
}
</style>
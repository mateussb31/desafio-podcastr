
<script setup lang="ts">
import Header from './components/Header.vue';
import Player from './components/Player.vue';
import Main from './components/Main.vue';
import Lancamentos from './components/Lancamentos.vue';
</script>

<template>
  <header>
    <Header></Header>
  </header>
  <main>
    <Lancamentos></Lancamentos>
    <Main></Main>
  </main>
  <aside>
    <Player></Player>
  </aside>
</template>

<style scoped>

</style>
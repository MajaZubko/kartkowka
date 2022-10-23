<template>
  <div class="app-container">
    <h1>Italiano Słowiano</h1>
    <InputSection v-for="text in textsToTranslate" :key="text" :text-to-translate="text" />
  </div>
</template>

<script>
import InputSection from "@/components/InputSection";
import textsToTranslate from './assets/data'

export default {
  name: 'App',
  components: {
    InputSection,
  },
  data() {
    return {textsToTranslate}
  }
}
</script>

<style>
body {
  margin: 0;
  padding: 0;
  overscroll-behavior: none;
}

.app-container {
  margin: 0;
  padding: 32px 0;
  display: flex;
  flex-direction: column;
  align-items: center;
  font-family: Arial;
  background: #fcbf49;
  color: #003049;
}
</style>

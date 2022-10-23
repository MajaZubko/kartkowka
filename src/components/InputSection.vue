<template>
  <div class="input-section">
    <span class="input-label">{{textToTranslate}}</span>
    <input />
  </div>
</template>

<script>
export default {
  name: 'InputSection',
  props: {
    textToTranslate: {
      type: String,
      default: ''
    }
  }
}
</script>

<style>
.input-section {
  display: flex;
  min-width: 40vw;
  margin-bottom: 8px;
}

.input-label {
  min-width: 20vw;
}

input {
  min-width: 20vw;
}
</style>

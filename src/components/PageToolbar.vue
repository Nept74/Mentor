<script setup>
import Button from './Button.vue'
</script>
<template>
  <div class="toolbar flex">
    <Button #button="meow"></Button>

  </div>
</template>

<style scoped>
.toolbar {
  background-color: white;
  border-bottom: 1px #edeae9af solid;
  width: 100%;
  height: 56px;
  padding: 0 24px;
}
</style>
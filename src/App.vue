<script setup>
import MarkdownEditor from './components/MarkdownEditor.vue';
</script>

<template>
  <markdown-editor></markdown-editor>
</template>

<style>
html, body, #app {
  width: 100%;
  height: 100%;
}

body {
  margin: 0;
}

#app {
  width: 800px;
  height: 500px;
  padding: 100px;
}
</style>

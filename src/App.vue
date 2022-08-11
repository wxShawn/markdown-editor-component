<script setup>
import { reactive } from 'vue';
import MarkdownEditor from './components/MarkdownEditor.vue';

const data = reactive({
  text: 'markdown text',
  html: 'html',
});

const handleDataChange = (data) => {
  console.log(data);
}
</script>

<template>
  <markdown-editor :data="data" @dataChange="handleDataChange"></markdown-editor>
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

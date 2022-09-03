<script setup>
import { ref } from 'vue';
import MarkdownEditor from './components/MarkdownEditor';

const handleDataChange = (data) => {
  // console.log(data);
}

const content = ref('');

const handleBtnClick = () => {
  console.log(content.value);
}
</script>

<template>
  <button @click="handleBtnClick">print content</button>
  <markdown-editor
    v-model:content="content"
    @dataChange="handleDataChange">
  </markdown-editor>
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

<template>
  <div class="page">
    <div class="card">
      <h1>{{ title }}</h1>
      <p>{{ message }}</p>
      <button @click="count++">你点击了 {{ count }} 次</button>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const title = 'Vue 3 示例项目'
const message = '这个项目可以先上传到 GitHub，再连接到 Codex。'
const count = ref(0)
</script>

<style scoped>
.page {
  min-height: 100vh;
  display: grid;
  place-items: center;
  background: #f5f7fb;
  font-family: Arial, sans-serif;
}

.card {
  width: 360px;
  padding: 24px;
  border-radius: 16px;
  background: white;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
  text-align: center;
}

h1 {
  margin-bottom: 12px;
  font-size: 28px;
}

p {
  margin-bottom: 20px;
  color: #666;
  line-height: 1.6;
}

button {
  border: none;
  border-radius: 10px;
  padding: 12px 18px;
  background: #42b883;
  color: white;
  font-size: 16px;
  cursor: pointer;
}
</style>

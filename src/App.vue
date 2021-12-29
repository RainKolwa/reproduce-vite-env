<script setup>
const env = JSON.stringify(import.meta.env);
const mode = import.meta.env.MODE;
const userNodeEnv = import.meta.env.VITE_USER_NODE_ENV;
const nodeEnv = import.meta.env.NODE_ENV;
</script>

<template>
  <pre>{{ env }}</pre>
  <h1>current mode: {{ mode }}</h1>
  <h1>userNodeEnv: {{ userNodeEnv }}</h1>
  <h1>nodeEnv: {{ nodeEnv }}</h1>
</template>

<style>
body {
  font-family: -apple-system, BlinkMacSystemFont, Helvetica Neue,
    PingFangSC-Regular, PingFang SC, Microsoft YaHei, Source Han Sans SC,
    Noto Sans CJK SC, WenQuanYi Micro Hei, sans-serif;
}
button,
a {
  @apply transition-colors duration-100;
}
.container {
  @apply px-4;
}
</style>

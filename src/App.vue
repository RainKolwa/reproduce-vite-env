<script setup>
const env = JSON.stringify(import.meta.env, undefined, 2);
const mode = import.meta.env.MODE;
const prod = import.meta.env.PROD.toString();
</script>

<template>
  <pre>{{ env }}</pre>
  <div>import.meta.<wbr />env.MODE: {{ mode }}</div>
  <div>import.meta.<wbr />env.PROD: {{ prod }}</div>
</template>

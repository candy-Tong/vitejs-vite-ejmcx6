<script setup>
import { ref } from 'vue';
//import 'vue-router';
//import 'lodash-es';

const count = ref(0);
setInterval(() => {
  count.value++;
}, 1000);
</script>

<template>
  <a-card title="antd title">
    <h2>将 import 'lodash-es'; 取消注释</h2>
    <h2>页面会刷新，count 会被重置</h2>
    <button>{{ count }}</button>
  </a-card>
</template>

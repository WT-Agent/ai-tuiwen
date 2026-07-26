<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 139****4422 生成了小红书美白精华爆款种草图文"
  },
  {
    "text": "用户 186****1199 获得了公众号故事化软文植入脚本"
  },
  {
    "text": "用户 131****8800 完成了人体工学椅幸福感测评推文"
  },
  {
    "text": "用户 158****3355 生成了小红书 10 万浏览量封面排版规范"
  },
  {
    "text": "用户 173****7711 取得了评论区求链接引导与私域引流 SOP"
  }
]);
</script>

<script setup lang="ts">
import { RouterView } from 'vue-router';
</script>

<template>
  <p>測試文字</p>
  <RouterView v-slot="{ Component }">
    <KeepAlive include="CitizenReportView">
      <component :is="Component" />
    </KeepAlive>
  </RouterView>
</template>

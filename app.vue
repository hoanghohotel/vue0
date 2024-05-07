<script setup lang="ts">
import { ConfigProvider } from 'radix-vue'

const useIdFunction = () => useId()
</script>

<template>
  <ConfigProvider :use-id="useIdFunction">
    <UiTooltipProvider>
      <NuxtLoadingIndicator color="hsl(var(--primary))" />
      <NuxtLayout>
        <NuxtPage />
      </NuxtLayout>
    </UiTooltipProvider>
  </ConfigProvider>
</template>

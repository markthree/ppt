<template>
    <n-badge :value="value" :max="30" type="info" :offset="[10, 0]">
        <slot />
    </n-badge>
</template>
  
<script setup lang="ts">
import { NBadge } from "naive-ui"

defineProps<{ value: number }>()
</script>
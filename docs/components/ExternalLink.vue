<script setup lang="ts">
defineProps<{
  href?: string
}>()
</script>

<template>
    <ULink :href="href" external rel="noopener" target="_blank" class="text-primary"><slot /> <UIcon name="i-lucide-external-link" class="size-3" /></ULink>
</template>

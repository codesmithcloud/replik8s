<script setup lang="ts">
defineProps<{
  text: string
}>()
</script>

<template>
    <UTooltip :text="text" :arrow="true" :delay-duration="0" :disable-closingtrigger="true">
        <TooltipText><slot /></TooltipText>
    </UTooltip>
</template>

<style scoped>
    span {
        text-decoration-line: underline;
        text-decoration-style: dotted;
        text-underline-position: under;
        text-decoration-color: var(--ui-secondary);
    }
    span:hover {
        cursor: help;
        text-decoration-color: var(--ui-primary);
    }
</style>

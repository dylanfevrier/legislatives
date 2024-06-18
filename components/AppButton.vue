<script setup lang="ts">
const props = defineProps<{label: string; variant: 'red' | 'black'}>();

const variant = `btn-${props.variant}`;
</script>

<template>
  <button class="btn" :class="variant">
    {{ props.label }}
  </button>
</template>

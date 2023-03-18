<template>
<button :type="type">
  <slot />
</button>
</template>

<script setup lang="ts">
withDefaults(defineProps<{
  type: 'submit' | 'reset' | 'button'
}>(), {
  type: 'submit'
})
</script>

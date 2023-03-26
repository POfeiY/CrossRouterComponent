<script setup lang="ts">
import { metadata } from '~/composables/floating'
// const props = defineProps<{
//   modelValue: 'string'
// }>()
const attrs = useAttrs()
metadata.attrs = attrs
// metadata.props = props
</script>
<template>
  <div />
</template>

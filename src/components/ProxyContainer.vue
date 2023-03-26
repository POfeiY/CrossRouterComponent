<script setup lang="ts">
import { metadata, proxyRef } from '~/composables/floating'
const el = ref()
const attrs = useAttrs()
metadata.attrs = attrs
onMounted(() => {
  proxyRef.value = el.value
})
// metadata.props = props
</script>
<template>
  <div ref="el" bg-gray-400:10 />
</template>

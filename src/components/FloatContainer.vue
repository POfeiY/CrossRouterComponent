<script setup lang="ts">
import type { StyleValue } from 'vue'
import { metadata, proxyRef } from '~/composables/floating'

// with native api
// watch(proxyRef, (el) => {
//   domRect.value = el?.getBoundingClientRect()
// }, { immediate: true })

const domRect = reactive(useElementBounding(proxyRef))

const style = computed<StyleValue>(() => ({
  transition: 'all .6s ease-in-out',
  position: 'fixed',
  top: `${domRect?.top ?? 0}px`,
  left: `${domRect?.left ?? 0}px`,
}))
</script>

<template>
  <div :style="style">
    <slot v-bind="metadata" />
  </div>
</template>

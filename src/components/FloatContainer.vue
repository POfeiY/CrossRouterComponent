<script setup lang="ts">
import { metadata } from '~/composables/floating'
</script>
<template>
  <slot v-bind="metadata" />
</template>

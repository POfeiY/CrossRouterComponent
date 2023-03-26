<script setup lang="ts">
let size = $ref(useLocalStorage('size', 120))
const enlarge = () => {
  size += 10
}
const delarge = () => {
  size -= 10
}
</script>
<template>
  <div flex="~ col" items-center justify="center">
    <div i-carbon-campsite text-4xl inline-block />
    <p>
      <span>PageA</span>
    </p>
    <div>
      <RouterLink to="/" btn>
        Back Index
      </RouterLink>
      <button btn m4 @click.stop="enlarge">
        bigger
      </button>
      <button btn @click.stop="delarge">
        smaller
      </button>
    </div>
    <ProxyContainer :style="{ width: `${size}px`, height: `${size}px` }" rounded="1/2" />
  </div>
</template>>

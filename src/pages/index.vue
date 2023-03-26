<script setup lang="ts">

</script>

<template>
  <div>
    <div i-carbon-campsite text-4xl inline-block />
    <p>
      <span>PageIndex</span>
    </p>
    <div>
      <RouterLink to="/PageA" class="btn m4">
        to PageA
      </RouterLink>
    </div>
    <ProxyContainer w-40 h-40 rounded-xl />
  </div>
</template>

<script setup lang="ts">
let toggle = $ref(false)
const switchHanle = () => {
  toggle = !toggle
}
</script>
<template>
  <div overflow-hidden transition="all .6s ease-in-out" @click="switchHanle">
    <img v-if="toggle"
      src="https://images.unsplash.com/photo-1679656127544-c4db649775cd?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=687&q=80">
    <img v-else
      src="https://images.unsplash.com/photo-1679499082480-a5a694a86ca1?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=687&q=80">
  </div>
</template>

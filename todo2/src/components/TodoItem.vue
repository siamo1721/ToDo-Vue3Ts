<script setup lang="ts">
const props = defineProps<{
  todo: {
    id: number
    title: string
    completed: boolean
  }
}>()
</script>

<template>
<li> {{props.todo.title}}</li>
  <li>{{props.todo.completed}}</li>
</template>

<style scoped>
li{
  background: aquamarine;
}
</style>
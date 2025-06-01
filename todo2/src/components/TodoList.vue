<script setup lang="ts">
import TodoItem from './TodoItem.vue';
const props = defineProps<{
  todos: {
    id: number
    title: string
    completed: boolean
  }[]
}>()
</script>

<template>
<div>
  <TodoItem
  v-for="todo in props.todos"
  key="todo.id"
  :todo="todo"
  />
</div>
</template>

<style lang="scss" scoped>
h1{
  color: aqua;
}
</style>
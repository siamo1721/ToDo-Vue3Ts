<script setup lang="ts">
import TodoList from "@/components/TodoList.vue";
import { ref } from "vue";

type Todo = {
  id: number
  title: string
  completed: boolean
}

const todos = ref<Todo[]>([
  { id: 1, title: 'первый', completed: false },
  { id: 2, title: 'второй', completed: false },
  { id: 3, title: 'третий', completed: false }
]);
</script>

<template>
  <TodoList :todos="todos"/>
</template>

<style scoped>

</style>
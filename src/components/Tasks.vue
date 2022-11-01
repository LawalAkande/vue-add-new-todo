<template>
  <Task :key="task.id" v-for="task of tasks" :task="task" />
</template>

<script>
import Task from "./Task.vue";
export default {
  name: "Tasks",
  components: {
    Task,
  },
  props: {
    tasks: Array,
  },
};
</script>

<style scoped></style>

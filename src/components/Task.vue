<template>
  <div :class="[task.reminder ? 'reminder' : '', 'task']">
    <h3>
      {{ task.text }} <span class="fas" @click="onDelete(task.id)">&#215;</span>
    </h3>
    <p>{{ task.day }}</p>
  </div>
</template>

<script>
export default {
  name: "Task",
  props: {
    task: Object,
  },
  methods: {
    onDelete(taskId) {
      console.log("the said task id: ", taskId);
    },
  },
};
</script>

<style scoped>
.fas {
  color: red;
}
.task {
  background: #f4f4f4;
  margin: 5px;
  padding: 10px 20px;
  cursor: pointer;
}
.task.reminder {
  border-left: 5px solid green;
}
.task h3 {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
</style>

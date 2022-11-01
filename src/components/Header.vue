<template>
  <header>
    <h1>{{ title }}</h1>
    <Button backgroundColor="green" text="Add Task" />
  </header>
</template>

<script>
import Button from "./Button.vue";

export default {
  name: "App",
  components: {
    Button,
  },
  props: {
    title: String,
  },
};
</script>

<style>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>

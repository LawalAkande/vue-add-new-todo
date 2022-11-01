<template>
  <button
    @click="onClick()"
    :style="{ 'background-color': backgroundColor }"
    class="btn"
  >
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "Button",
  props: {
    backgroundColor: String,
    text: String,
  },

  methods: {
    onClick() {
      console.log("Hello boss");
    },
  },
};
</script>

<style scoped></style>

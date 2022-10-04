<template>
  <header>
    <h1>{{ title }}</h1>
    <Button text="Add Task" color="green" />
  </header>
</template>

<script>
import Button from "./Button.vue";

export default {
  name: "Header",
  // ways to setup props
  //   props: ["title"], // 1
  //   props: {          // 2
  //     title: String
  //   }
  // 3rd way with default and specifiity
  props: {
    title: {
      type: String,
      default: "Header",
    },
  },
  components: {
    Button,
  },
};
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>

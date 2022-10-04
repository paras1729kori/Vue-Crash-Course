<template>
  <button @click="onClick" :style="{ background: color }" className="btn">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "Button",
  props: {
    text: String,
    color: String,
  },
  methods: {
    onClick() {
      comsole.log("click");
    },
  },
};
</script>

<template>
  <h1>I am .Net developer</h1>
  <p>
    which always wants to improve skills and works with the newest technologies
  </p>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  data() {
    return {
      msg: "example" as string,
      dataFromApi: "" as string,
    };
  },
  methods: {},
});
</script>

<style scoped></style>

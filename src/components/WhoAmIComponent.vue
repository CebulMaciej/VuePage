<template>
  <div id="whoAmI">
    <h1>I am .Net developer,</h1>
    <p>
      which main goal is improving skills and works with the latest technologies
    </p>
  </div>
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

<style scoped>
#whoAmI {
  margin-bottom: 5rem;
}
</style>

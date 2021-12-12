<template>
  <div class="ability">
    <h1>{{ header }}</h1>
    <div>
      {{ content }}
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  props: {
    header: String,
    content: String,
  },

  data() {
    return {};
  },
  methods: {},
});
</script>

<style scoped>
.ability p {
  max-width: 50%;
  display: block;
  margin: auto;
}
.ability div {
  max-width: 50%;
  display: block;
  margin: auto;
}
</style>

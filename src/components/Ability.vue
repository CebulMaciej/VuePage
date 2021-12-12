<template>
  <div class="ability col-xs-12 col-sm-12 col-md-6 col-12">
    <h2>{{ header }}</h2>
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
.ability {
  padding: 15px 20px;
}
</style>

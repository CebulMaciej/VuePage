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
  margin-bottom: 2rem;
}
.ability div {
  padding: 15px 20px;
  background: #dcdde1;
  border-radius: 1px 15%;
}
h2 {
  border-bottom: 1px solid #000000;
}
</style>

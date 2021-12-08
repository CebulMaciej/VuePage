<template>
  <button @click="clicked">{{ msg }}</button>
  <div>{{ dataFromApi }}</div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

interface Book {
  name: string;
}

class Paper implements Book {
  name: string;

  constructor(name: string) {
    this.name = name;
  }
}

export default defineComponent({
  data() {
    return {
      book: Paper as Book,
      msg: "example" as string,
      dataFromApi: "" as string,
    };
  },
  methods: {
    async clicked() {
      let tmp = await this.getDataFromApi();
      this.dataFromApi = tmp;
      this.book = new Paper(tmp);
    },

    async getDataFromApi() {
      const response = await fetch("https://api.maciejcebula.net");
      return await response.text();
    },
  },
});
</script>

<style scoped></style>

<template>
  <MyFirstComponent></MyFirstComponent>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import MyFirstComponent from "@/components/MyFirstComponent.vue"; // @ is an alias to /src

@Options({
  components: {
    MyFirstComponent,
  },
})
export default class MyFirstPage extends Vue {}
</script>

<style scoped></style>

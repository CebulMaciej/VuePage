<template>
  <div id="whoAmI" class="container-fluid">
    <div class="row">
      <div class="aboutMe col-12 col-md-6">
        <h1>Hi there,</h1>
        <h1 class="name">I'm Maciej Cebula</h1>
        <h4>.Net Developer,</h4>
        <h5>
          whose main goal is to improve skills and to work with the latest
          technologies
        </h5>
      </div>
      <div class="photoDiv col-12 col-md-6"></div>
    </div>
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
  background: #b9b9b9;
}
.aboutMe {
  padding-top: 230px;
  padding-bottom: 230px;
}
.aboutMe .name {
  font-size: xxx-large;
  font-weight: bolder;
}
.photoDiv {
  background-image: url("../assets/doge.png");
  background-size: 600px;
  width: 600px;
  height: 600px;
  margin: auto;
}
</style>

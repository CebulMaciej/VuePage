<template>
  <div class="abilities">
    <Ability
      header="Writing systems from scratch"
      content="I'm able to preparing architecture for solutions matching to the
      requirements. All my solutions are served as docker containers, which can
      be deployed on any server or ochestrating tool like Kubernetes."
    >
    </Ability>

    <Ability
      header="Rewriting systems from legacy technologies"
      content="If your system has been written in old technologies and your technological
      debt is too big, probably this is time to rewrite application to new
      technologies which are in LTS version or just supported."
    >
    </Ability>

    <Ability
      header="Building CI/CD processes"
      content="Deploying solutions after every change is just waste of time. If something
      could be automated, it should be done. I'am able to writing pipeline which
      can build application, build docker image and then push it to the remote
      repository. And after push just deploy it on destination machine. I have
      written script for Kubernetes, applications containerized in remote VPS or
      just on VPS, without containerization."
    >
    </Ability>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Ability from "./Ability.vue";

export default defineComponent({
  components: {
    Ability,
  },
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
.abilities {
  text-align: center;
  align-items: center;
}
.abilities p {
  max-width: 50%;
  display: block;
  margin: auto;
}
.abilities div {
  max-width: 50%;
  display: block;
  margin: auto;
}
</style>

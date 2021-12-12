<template>
  <div class="abilities container-fluid">
    <h1>What services I provide:</h1>
    <div class="row">
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
    </div>
    <div class="row">
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

      <Ability
        header="Creating frontent page (in progress)"
        content="I'm still learning new technologies and new abilities, writing frontends is one of my current goals. For now, i'm writing this page using Vue.js 3 with TypeScript. In the future i will able to do it for you and your company."
      >
      </Ability>

      <Ability
        header="Configuring machines for applications"
        content="I work a lot with linux machines, because this is my current OS on every device, i'm able to configure VPSs for being machine for application or i can help with configuring Azure deployments"
      >
      </Ability>

      <Ability
        header="Helping with app containerisation"
        content="Containerization for me is more than ability or skill. This is very helpful tool which make possible run application everywhere. This topic is my cup of tea."
      >
      </Ability>
    </div>
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
  margin-top: 5rem;
  text-align: center;
  align-items: center;
  width: 90%;
}
</style>

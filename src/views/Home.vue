<template>
  <div class="home">
    <WhoAmIBigComponent></WhoAmIBigComponent>
    <WhatICanDo></WhatICanDo>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import WhoAmIComponent from "@/components/WhoAmIComponent.vue"; // @ is an alias to /src
import WhatICanDo from "@/components/WhatCanIDo.vue"; // @ is an alias to /src
import WhoAmIBigComponent from "@/components/WhoAmIBigComponent.vue";

@Options({
  components: {
    WhoAmIComponent,
    WhatICanDo,
    WhoAmIBigComponent,
  },
})
export default class Home extends Vue {}
</script>
<style>
.home {
  margin: auto;
}
</style>

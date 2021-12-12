<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <WhoAmIComponent></WhoAmIComponent>
    <WhatICanDo></WhatICanDo>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import WhoAmIComponent from "@/components/WhoAmIComponent.vue"; // @ is an alias to /src
import WhatICanDo from "@/components/WhatCanIDo.vue"; // @ is an alias to /src

@Options({
  components: {
    WhoAmIComponent,
    WhatICanDo,
  },
})
export default class Home extends Vue {}
</script>

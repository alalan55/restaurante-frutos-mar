<template>
<div class="container">
  <CapaTemplate />
  <SobreTemplate/>
</div>

</template>

<script>
import { CapaTemplate, SobreTemplate } from "@/components/templates";

export default {
  name: "App",
  components: {
    CapaTemplate,
    SobreTemplate
  },
};
</script>
<style lang="scss" scoped>

</style>
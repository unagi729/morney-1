<template>
  <div>
    <svg class="icon" @click="$emit('click',$event)">
      <use :xlink:href="'#'+name" />
    </svg>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

const importAll = (requireContext: __WebpackModuleApi.RequireContext) =>
  requireContext.keys().forEach(requireContext);
try {
  importAll(require.context("../assets/icons", true, /\.svg$/));
} catch (error) {
  console.log(error);
}

export default Vue.extend({
  props: ["name"]
});
</script>

<style lang="scss" scoped>
.icon {
  width: 2em;
  height: 2em;
  vertical-align: -0.15em;
  fill: currentColor;
  overflow: hidden;
}
</style>
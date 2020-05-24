<template>
  <div class="nav-wrapper">
    <div class="content">
      <slot />
    </div>
    <Nav />
  </div>
</template>

<script lang="ts">
import Vue from "vue";
export default Vue.extend({
  name: "Layout"
});
</script>

<style lang="scss" scoped>
.nav-wrapper {
  display: flex;
  border: 1px solid green;
  flex-direction: column;
  height: 100vh;
}
.content {
  flex-grow: 1;
  overflow: auto;
}
</style>
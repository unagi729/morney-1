<template>
  <Layout>编辑标签</Layout>
</template>

<script lang="ts">
import Vue from "vue";
import { Component } from "vue-property-decorator";

@Component
export default class EditLabel extends Vue {
  created() {
    const id = this.$route.params.id;
  }
}
</script>

<style lang="scss" scoped>
</style>